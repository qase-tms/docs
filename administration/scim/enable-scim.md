# Enable SCIM

SCIM API is enabled for all customers with Enterprise subscription by default. To manage users with SCIM in your Qase Enterprise account you will need to create a new API token:

1. Navigate to **Workspace > SCIM** page:

<figure><img src="../../.gitbook/assets/Screenshot 2023-11-06 at 10.56.23 AM (1).png" alt=""><figcaption></figcaption></figure>

2. Now you can create a new SCIM API Token.

<figure><img src="../../.gitbook/assets/Screenshot 2023-11-06 at 10.56.28 AM.png" alt=""><figcaption></figcaption></figure>

3. To ensure that everything is working as expected you can make the following request:\
   `GET: https://app.qase.io/scim/v2/Users`\
   Request Headers:\
   `Accept` _application/scim+json_\
   `Content-Type` _application/json_\
   `Authorization` _Bearer + API Token from the previous step_

> 📘
>
> Base URL and Authorization type
>
> As you can see from the previous example the base URL for SCIM API is _https://app.qase.io/scim/v2/Users_.\
> The API token must be included in every call to SCIM via **Authorization** header with type **Bearer**

> 🚧
>
> HTTPS protocol
>
> We support **HTTPS** requests only. Requests to **HTTP** protocol are redirected to **HTTPS** - please note that this redirection response can be handled incorrectly by certain tools.

curl example

```curl
curl -H "Accept: application/json" -H "Content-Type: application/json" -H "Authorization: Bearer <token>" https://app.qase.io/scim/v2/Users
```
