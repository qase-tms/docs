# Jenkins

### What is Jenkins?

Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration and continuous delivery. It is a server-based system that runs in servlet containers.

### Why use Jenkins integration?

Qase integration for Jenkins allows you to start your automated runs directly from Qase, without the need to go to Jenkins to set them up separately.

### How to install Jenkins? <a href="#h_29ba35be48" id="h_29ba35be48"></a>

1. Log into your Jenkins instance.
2. Create a Jenkins API token and copy it.
3. Go to the apps page in Qase.
4.  Choose Jenkins app:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705068961/11a10bd6b41101e09f630a64/Untitled+(15).png" alt=""><figcaption></figcaption></figure>
5.  Click the “Install now” button:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705069373/690cf4f9c37b44355c20899b/Untitled+(16).png" alt=""><figcaption></figcaption></figure>
6. Input your data in the form and press the “Install” button.

### Usage <a href="#h_511df78dc7" id="h_511df78dc7"></a>

1. Go to the Test Runs page.
2. Click the “Start new test run” button
3.  Select "Automated" test run to be created:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705071104/ddb1e58a947740c0ba2fb329/Untitled+(18).png" alt=""><figcaption></figcaption></figure>
4.  Select Jenkins CI/CD system:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705071410/83fa2e2116e8a5b36af3d739/Untitled+(19).png" alt=""><figcaption></figcaption></figure>
5.  Then choose a "Job", which you want to start and fill in other parameters:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705071625/ba330a20609aeceb4e89d0d3/Untitled+(20).png" alt=""><figcaption></figcaption></figure>
6. Start the test run

You can observe the pipeline status:

<figure><img src="https://downloads.intercomcdn.com/i/o/705072043/660e9836aa3be8fd6b49ed97/Untitled+(21).png" alt=""><figcaption></figcaption></figure>

...and the pipeline result:

<figure><img src="https://downloads.intercomcdn.com/i/o/705072437/b639291d38d562071363da42/Untitled+(22).png" alt=""><figcaption></figcaption></figure>

#### How to use Jenkins with Qase reporters? <a href="#h_e8b120b92f" id="h_e8b120b92f"></a>

1. Prepare a job that runs your tests.
2. Configure a Qase reporter for your testing framework.
3.  Make your job parameterized:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705073289/38a3c5544cccfa5f804936e9/Untitled+(23).png" alt=""><figcaption></figcaption></figure>
4. Add string parameters for the Qase reporter. They will be used to link test results with automated test runs and they will be filled in by Qase automatically:
   * QASE\_PROJECT\_CODE
   * QASE\_RUN\_ID
   * QASE\_REPORT
   * QASE\_RUN\_COMPLETE
   * QASE\_API\_BASE\_URL
5. Go to the Apps page on Qase, then activate and generate a new token for reporter app. You can also use regular (user-issued) API tokens.
6. Save created token as credentials in Jenkins: [https://www.jenkins.io/doc/book/using/using-credentials/#adding-new-global-credentials](https://www.jenkins.io/doc/book/using/using-credentials/#adding-new-global-credentials)
7.  Configure your job to pass saved token in QASE\_API\_TOKEN environment variable:



    <figure><img src="https://downloads.intercomcdn.com/i/o/705074174/55dc555d9dabdb55cefc9d4d/Untitled+(24).png" alt=""><figcaption></figcaption></figure>
8.  You can also use the pipeline plugin. Example is below:

    ```
    pipeline {
        agent {
            kubernetes {
              yaml '''
              spec:
                containers:
                - name: node
                  image: node:16.14.2-alpine3.15
                  command:
                  - sleep
                  args:
                  - 99d
    '''
            }
        }
        parameters {
            string(name: 'QASE_PROJECT_CODE')
            string(name: 'QASE_RUN_ID')
            string(name: 'QASE_REPORT')
            string(name: 'QASE_RUN_COMPLETE')
            string(name: 'QASE_API_BASE_URL')
            credentials(name: 'QASE_API_TOKEN', credentialType: "Secret text")
        }
        environment { 
            QASE_API_TOKEN = credentials("${params.QASE_API_TOKEN}") 
        }
        stages {
            stage('Run tests') {
                steps {
                    git url: 'https://github.com/foo/bar.git', branch: 'main'
                    container('node') {
                        sh 'npm i'
                        sh 'npx jest'
                    }
                }
            }
      }
    }
    ```
