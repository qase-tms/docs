# OneLogin

### How to configure SSO with OneLogin?

To set up your Qase account with SSO/SAML and OneLogin, you'll need to take the following steps:

1\. Sign in to the OneLogin admin panel and go to the "Applications" section.

2\. Click on the button "Add app"

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827502/82a5af8f5767d96594b92126/Screenshot_2020-07-24_at_00.44.25.png" alt=""><figcaption></figcaption></figure>

3\. Type "Qase" in a search box and press "Enter". You will see an app in the list - click on it.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827522/a7693df1d7c884dfef93924f/Screenshot_2020-07-24_at_00.47.22.png" alt=""><figcaption></figcaption></figure>

4\. You will see a form with pre-filled values. You can change some details if you want. When you are ready, click on the "Save" button.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827536/13c7e1f54f8e658f2e87d0e2/Screenshot_2020-07-24_at_00.48.28.png" alt=""><figcaption></figcaption></figure>

5\. Go to the "SSO" tab and copy the values from the "Issuer URL" and "SAML 2.0 Endpoint" fields. We will use them to link Qase with OneLogin.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827550/1daa063a3b48153e1c0797d8/Screenshot_2020-07-24_at_00.48.52.png" alt=""><figcaption></figcaption></figure>

6\. Click on the "View Details" link under the "X.509 Certificate" field, you will see a page with certificate details. Copy "X.509 Certificate" details from the textarea:

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827558/c06d50ca7b08e0b32ff2cb1d/Screenshot_2020-07-24_at_00.50.03.png" alt=""><figcaption></figcaption></figure>

7\. OneLogin setup is complete. Now you need to go to the Qase security page and link your account with OneLogin's credentials. Click on the "Enable SSO/SAML" toggle button and fill the form:

* _SAML Sign-in URL:_ paste "SAML 2.0 Endpoint" from step 5.
* _Identity Provider Issuer:_ paste "Issuer URL" from step 5.
* _Key x509 Certificate:_ paste "X.509 Certificate" from step 6.
* _Domains:_ provide a list of domains separated by a comma, that will be used for SSO. Public domains like gmail, hotmail, and etc are not allowed.
* _Default role:_ choose a default role that will be granted to the new users.

If you want new users who join your team to become a read-only by default, check "Automatically add new users as read-only members" checkbox.

After the form is filled, click on the "Save" button.

<figure><img src="https://qase.intercom-attachments-1.com/i/o/387827563/986c7fa88a469e2808bf26f0/qase_sso_setup.png" alt=""><figcaption></figcaption></figure>

The setup is complete. Now you can logout from the app and log in through the SSO login form.
