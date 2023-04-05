# AzureAD

### How to configure SSO with AzureAD?

1\. Sign in to the admin console of your AzureAD account.

2\. Click on "Azure Active Directory" icon:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827399/3461fa8567e223aeef8f0687/Screenshot_2020-08-19_at_20.29.11.png" alt=""><figcaption></figcaption></figure>

3\. Go to "Enterprise applications" section and click on "New application" button:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827405/05819d3f17f9f032f4358f35/Screenshot_2020-08-19_at_20.30.45.png" alt=""><figcaption></figcaption></figure>

4\. Choose "Non-gallery application":

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827415/82e44dc9e9324e19ace33ec3/Screenshot_2020-08-19_at_20.34.18.png" alt=""><figcaption></figcaption></figure>

5\. Name your application (e.g. Qase) and click on "Add" button:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827420/45615770c4283508eddf6d07/Screenshot_2020-08-19_at_20.35.01.png" alt=""><figcaption></figcaption></figure>

6\. Click on "Set up single sign on":

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827439/46c207afc1859ec218e17276/Screenshot_2020-08-19_at_20.37.38.png" alt=""><figcaption></figcaption></figure>

7\. Choose "SAML":

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827445/8ed1feb194fc6336a2630e68/Screenshot_2020-08-19_at_20.39.33.png" alt=""><figcaption></figcaption></figure>

8\. Now, you need to set up your AzureAD application. Click on the "Edit" button in the "Basic SAML Configuration" block. And fill the form with the following data:

* Identifier (Entity ID): [https://app.qase.io/saml/metadata](https://app.qase.io/saml/metadata)
* Reply URL (ACS URL): [https://app.qase.io/saml/acs](https://app.qase.io/saml/acs)
* Sign on URL: [https://app.qase.io/sso/login](https://app.qase.io/sso/login)

When you are ready, click on "Save" button.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827458/47e6cfeab4b9bd921ae2b67f/Screenshot_2020-08-19_at_20.55.58.png" alt=""><figcaption></figcaption></figure>

9\. Now you need to configure attribute mapping. Click on "Edit" button in "User Attributes & Claims" section and for "Required claim" set Name ID format to _persistent_ and Name ID value to _user.mail._

Also, add two new claims:

* fname: user.givenname
* lname: user.surname

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827470/02e5084ea49ad4bb50d0ec90/Screenshot_2020-08-20_at_00.58.15.png" alt=""><figcaption></figcaption></figure>

10\. Now, you are ready to set up SSO on the Qase side. But at first, you need to get data from the AzureAD app:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827483/5adde1ef3f6ffbd2b28edf41/Screenshot_2020-08-19_at_21.17.16.png" alt=""><figcaption></figcaption></figure>

1. Download the certificate (Base64)
2. Copy Login URL
3. Copy Azure AD identifier

10\. Now you need to go to the Qase [security page](https://app.qase.io/team/security) and link your account with AzureAD credentials. Click on the "Enable SSO/SAML" toggle button and fill the form:

* _SAML Sign-in URL:_ paste login URL from the previous step
* _Identity Provider Issuer:_ paste Azure AD identifier from the previous step
* _Key x509 Certificate:_ open downloaded in the previous certificate in any editor, copy its content, and paste in the textarea.
* _Domains:_ provide a list of domains separated by a comma, that will be used for SSO. Public domains like gmail, hotmail, and etc are not allowed.
* _Default role:_ choose a default role that will be granted to the new users.

If you want new users who join your team to become a read-only by default, check "Automatically add new users as read-only members" checkbox.

After the form is filled, click on the "Save" button.

\
