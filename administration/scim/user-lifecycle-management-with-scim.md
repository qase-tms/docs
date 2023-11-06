---
description: Learn about managing user access with the Qase SCIM API.
---

# User lifecycle management with SCIM

Any organization that grants access to its services and that uses permissions to control how users engage must manage users and their access. This lifecycle starts when a company onboards its users and continues until they leave the company. Managing users and their access involves various systems and can become challenging.

The increasing use of APIs for nearly every system has enabled organizations to automate the provisioning and management of users, often using the [System for Cross-domain Identity Management (SCIM)](https://en.wikipedia.org/wiki/System\_for\_Cross-domain\_Identity\_Management) as a standard. SCIM provides API methods and JSON objects that define users and groups, so identity providers and integration tools can manage users across systems.

This article looks into the Qase SCIM API, its capabilities, and some standard processes to consider when implementing automatic provisioning and management of users in Qase.

### Qase SCIM API overview

The Qase SCIM API enables organizations to manage user access automatically. It uses an identity provider, and it includes an interface for other identity providers that support the SCIM protocol. The documentation already features several walkthroughs for configuring an Okta or Azure Active Directory (AD) instance. An Okta or AD instance enables the automatic provisioning of users, and it controls access for teams aligned with the two identity providers.

Additionally, you can call the SCIM API independently for greater control and customization. Independently calling the SCIM API allows middleware to create, update, and delete users.

### User lifecycle management with the Qase SCIM API

Understanding the information a company uses for onboarding and as users transition into new roles enables you to use your systems and data efficiently. Let's explore some common scenarios organizations encounter when implementing automated user management. We can then understand how the Qase SCIM API can assist with automating the user journey.

Suppose an organization has connected a single sign-on (SSO) capability for Qase logins, but uses an integration platform to perform the SCIM actions. This example demonstrates how to use the API in standard processes, such as onboarding new users and offboarding users.

### New user onboarding

When discussing automated user management, one of the first topics tends to be creating new users in an application. Here, the ideal user experience is one in which account creation provides immediate access to all necessary resources.

For this example organization, when a company adds a new user to the `qaseUsers` group, the integration layer first calls the SCIM Users API to look up the user, using filters to ensure that the user doesn’t already exist in the system. For a user with the email `alex.smith@example.com`, the lookup would look like this:

```html
https://app.qase.io/scim/v2/Users?attributes=name,userName&filter=(userName eq "alex.smith@example.com")
```

If the user doesn’t exist, the integration layer calls the create method with the user’s details. This method only requires the username (the Qase email address), a family name, and a given name. You can also save the user ID with a property in your user directory to ensure that you have correctly linked the users.

### User offboarding and deletion

Finally, when a user leaves your organization or no longer requires Qase, you must clean up their accounts. Of course, you can use the Delete User API to delete the account.\
However, in cases where the user no longer requires Qase, or if policies require that user accounts remain, you can also set the user’s status to inactive using the Update user API.

### Conclusion

The Qase SCIM API provides all the necessary components for managing your organization’s users through the entire lifecycle. Using existing user information and security groups or roles can make Qase's user and group management almost entirely automated.
