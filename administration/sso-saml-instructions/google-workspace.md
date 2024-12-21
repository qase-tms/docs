# Google Workspace

### How to configure SSO with Google Workspace?

To set up your Qase account with SSO/SAML and Google Workspace, you'll need to take the following steps:

1\. Sign in to the [Admin Console](https://support.google.com/a/answer/182076) of your Google Workspace account. You'll need to be a G Suite account administrator

2\. Click through the "Apps - Manage apps and their settings" icon:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827588/7fd27dfdd9847d0902f407f7/Screenshot_2020-07-15_at_01.07.26.png" alt="" width="563"><figcaption></figcaption></figure>

3\. Click on "SAML Apps":

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827598/7c08b73c4b6ffa136897125b/Screenshot_2020-07-15_at_01.08.00.png" alt="" width="563"><figcaption></figcaption></figure>

4\. Click on the yellow plus button on the bottom right to add a new app:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827612/94ab2d6c1b2f5b7c7856dcfb/Screenshot_2020-07-15_at_01.09.23.png" alt="" width="563"><figcaption></figcaption></figure>

5\. In "Step 1", click on "Setup my own custom app" on the bottom:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827626/5e68599a8b1b1a23fef9f4d4/Screenshot_2020-07-15_at_01.11.12.png" alt="" width="563"><figcaption></figcaption></figure>

6\. Copy the "SSO URL", "Entity ID" and download the "Certificate". We will use them in the next steps. Click on the "Next button".

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827649/2e16ece3c3adfe3512d35e7c/Screenshot_2020-07-15_at_01.11.53.png" alt="" width="563"><figcaption></figcaption></figure>

7\. Fill the form with the application name and description. We suggest using "Qase" as the name of the app - it will be easier to find it in the future. Also, you can upload a logo. After the form is complete, click on the "Next" button.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827669/c2f5bc608e9b43f41c6008fc/Screenshot_2020-07-15_at_01.12.36.png" alt="" width="563"><figcaption></figcaption></figure>

8\. On this step, you will need to fill the form with the following details:

* _ACS URL:_ [https://app.qase.io/saml/acs](https://app.qase.io/saml/acs)
* _Entity ID:_ [https://app.qase.io/saml/metadata](https://app.qase.io/saml/metadata)
* _Start URL:_ [https://app.qase.io](https://app.qase.io)
* _Signed Response:_ Checked
* _Name ID:_ Basic Information / Primary Email
* _Name ID Format:_ EMAIL

After you fill the form with necessary data, click on the "Next" button.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827684/032bebd0d6ac7d3dda8cd1ab/Screenshot_2020-07-15_at_01.13.31.png" alt="" width="563"><figcaption></figcaption></figure>

9\. If you want to save the user's first name, last name, and job title in Qase, you need to add attribute mapping fields. That can be done by clicking on the "Add new mapping" button and selecting the values like on this screenshot:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827696/b401ae5c57545079c5524843/Screenshot_2020-07-15_at_01.14.19.png" alt="" width="563"><figcaption></figcaption></figure>

10\. Google setup is complete. Now you need to go to the Qase [security page](https://app.qase.io/team/security) and link your account with Google's credentials. Click on the "Enable SSO/SAML" toggle button and fill the form:

* _SAML Sign-in URL:_ paste SSO URL from step 6.
* _Identity Provider Issuer:_ paste EntityID from step 6.
* _Key x509 Certificate:_ open downloaded in step 6 certificate in any editor, copy its content, and paste in the textarea.
* _Domains:_ provide a list of domains separated by a comma, that will be used for SSO. Public domains like gmail, hotmail, and etc are not allowed.

`Any domains that are added will need to be verified. To do so, you will need to add a TXT record to the domain's DNS records.`

<figure><img src="../../.gitbook/assets/Kapture 2024-09-21 at 10.41.38.gif" alt="" width="563"><figcaption></figcaption></figure>

* _Default role:_ choose a default role that will be granted to the new users.

If you want new users who join your team to become a read-only by default, check "Automatically add new users as read-only members" checkbox.

After the form is filled, click on the "Save" button.



Setup is complete. Now you can logout from the app and log in through the SSO login form.
