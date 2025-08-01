The password field for the login form of the application reveals the password in plaintext. An attacker with local access can shoulder surf or otherwise tailgate a user and watch them log in to the application. From here, an attacker could log in as a user to impersonate them or make requests on their behalf.

**Business Impact**

This vulnerability can lead to reputational damage and indirect financial loss to the company through the impact to customers’ trust.

**Steps to Reproduce**

1. Use a browser to navigate to: {{URL}}
1. Enter text within the password field
1. Use the `Inspect` tool to see that the input is shown in plaintext

{{screenshot}}

**Proof of Concept (PoC)**

The screenshot(s) below demonstrate(s) the vulnerability:
>
> {{screenshot}}
