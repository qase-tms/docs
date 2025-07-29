# Okta

{% hint style="info" %}
If you want to setup SSO along with SCIM (user provisioning), [jump to this section.](okta.md#h_b042f13c2e)
{% endhint %}

## SSO (SAML) Setup:

To set up your Qase account with SSO/SAML and Okta, you'll need to take the following steps:

1\. Login to your Okta Admin dashboar

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

2\. Go to Applications and click on "Browse App Catalog"

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

3\. Search for "Qase"

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

4\. Click on "Add Integration

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

5\. Check on the option for "Do not display application icon to users" and click "Done"

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

6\. Once activated, go to the "Sign On" tab, and on the lower left, click "View SAML setup instructions".

<figure><img src="../../.gitbook/assets/image (6) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

7\. This will take you to another page where you will find your SAML Sign-In URL, Identity Provider Issuer, and your Key x509 Certificate and further instructions on how to add these to Qase.



8\. Google setup is complete. Now you need to go to the Qase [security page](https://app.qase.io/workspace/security) and link your account with Google's credentials. Click on the "Enable SSO/SAML" toggle button and fill the form

<figure><img src="../../.gitbook/assets/33292.png" alt="" width="563"><figcaption></figcaption></figure>

* Map the following parameters as shown in the screenshot above.
* SAML Sign-in URL
* Identity Provider Issuer
* Key x509 Certificate
*   Domains\*: provide a list of domains separated by a comma, that will be used for SSO. Public domains like Gmail, Hotmail, etc. are not allowed.\
    \
    \*_This step is mandatory._\


    `Any domains that are added will need to be verified. To do so, you will need to add a TXT record to the domain's DNS records`

<figure><img src="../../.gitbook/assets/Kapture 2024-09-21 at 10.41.38.gif" alt="" width="563"><figcaption></figcaption></figure>

9\. If you want new users who join your team to become a read-only by default, check "Automatically add new users as read-only members" checkbox.

After the form is filled, click on the "Save" button.

Setup is complete. Now you can logout from the app and log in through the [SSO login form.](https://app.qase.io/sso/login)



## Setting up SCIM for User Provisioning and De-provisioning <a href="#h_b042f13c2e" id="h_b042f13c2e"></a>

With SCIM, the IdP will automatically create, update and delete users on Qase when you modify them on the IdP.

The Qase app on the Okta appstore doesn't support the SCIM features, so we'll need to set up a custom app if you need the SCIM feature.

From the Admin console, choose 'Applications' and then, click 'Create App Integration'

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642568195/aef0b85d7394e47c1266473a1335/image.png?expires=1753876800&#x26;signature=762a69c6b358be43c1471d37bed1e304dae21c53e7bdfbbd37c9100227b6529c&#x26;req=dSYjFMx4lYBWXPMW3nq%2BgcmRZbB89k3FrWWr9Z65OllYglaGJGNPuL3qFQ6S%0Aptwndn%2BQlI%2FRA0aKFz9cL2Hljyw%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Choose 'SAML 2.0'

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642569668/d2a801754eb0ccc8bd10ea095be5/image.png?expires=1753876800&#x26;signature=71f938401419930aceeccf9c4641855b643a6e6f2b19e0032c1277828eba91e7&#x26;req=dSYjFMx4lIdZUfMW3nq%2BgUxtdKgMuqShq4ez1mwMeUT3SAFDkv5JzyjC84IB%0AD%2FIdK5R62TYT9ddC8EohnLR7m3E%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

On the next page, provide a name for this app and continue to Step 2.

Fill out the following details:

1. Single sign-on URL: [https://app.qase.io/sso/login](https://app.qase.io/sso/login) _(we can use this value for the receipient and destination URL)_
2. Audience URI (SP Entity ID): [https://app.qase.io/saml/metadata](https://app.qase.io/saml/metadata)
3. NameID format: `persistent`
4. Application username: `Okta username`

Once the app is created, you'll need to go to the General tab and check the SCIM option.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642697949/f270b2da7b94b9241267b06096b7/image.png?expires=1753876800&#x26;signature=a0690a0547fc8f2949cfa65e5129b06e3c3f3289f4e0c6b77dafc9625accb6d5&#x26;req=dSYjFM93mohbUPMW3nq%2Bgbmh6CNw5ZW603b%2BWkiR2rTIUAkoPYufbxC92Iua%0At6JCEnaYzal3MocmspV1ryVS6WU%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

When you enable the SCIM option, you'll see a new tab that says - 'Provisioning'. Here, you'll need to enter the following info:

1. SCIM connector base URL: `https://app.qase.io/scim/v2/`
2. Unique identifier field for users: `email`
3. Check the first three options (Currently, Qase SCIM API doesn't support Groups provisioning)
4. Select Authentication mode as `HTTP Header`
5. In this field, enter the SCIM token generated from: [https://app.qase.io/workspace/scim](https://app.qase.io/workspace/scim)

You can test the connector configuration to check if everything is right.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642699350/6df34c4eb00f1f5d1379bd97178d/image.png?expires=1753876800&#x26;signature=bca479ee6084cc4587fc69f039859e225d7bfc70e1c0cde0dc8a976f0bc25bad&#x26;req=dSYjFM93lIJaWfMW3nq%2BgU2dUs%2Fm4bUlSJDmUamvAdOYYignC1nJHCt4Zuqh%0A5%2BreK5%2Bt%2F0WN1QSuWa0RZ9aJzcE%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Once the connection is tested to be working successfully, enable the following options from the 'To app' section –

1. Create Users
2. Update User Attributes
3. Deactivate Users

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642697133/37462c7042451460e1e805fbd822/image.png?expires=1753876800&#x26;signature=56d7a2c336c437cc155d7b832a133277c4acb7b0f62c831f7dbbf8bd53ce9300&#x26;req=dSYjFM93moBcWvMW3nq%2BgdSY0ocFaItiJ%2F7%2FVmX5ugHOuqV9LeDsijqzVZ4N%0A9g9PEFEid0ajDicrjOPCkdv%2FJx0%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

That's it, you've successfully configured SCIM for Qase with Okta. You can set up the SSO on this app, from the Sign-on tab.

For the data that you'll need to set up on Qase, follow this link and the instructions on the landing page.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1642705781/a27a041ef9b73381b11c48ccb915/image.png?expires=1753876800&#x26;signature=6af964ce7eaa0d091c664acad49e69a68e194b226c9871ccc8cad1bc1e6c6300&#x26;req=dSYjFM5%2BmIZXWPMW3nq%2BgQwmr9rhy3cOO5L74%2ByBvH1YsRccZVqW6dPqAeZi%0AASLpbwprQLF9H941YNDrDus%2Fbn4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
IdP initiated login is **not** supported.

Users will have to sign-in from this Qase's SSO Login page: [https://app.qase.io/sso/login](https://app.qase.io/sso/login)
{% endhint %}
