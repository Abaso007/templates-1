The user’s password is kept in memory after the application has ceased utilizing it. An attacker can abuse this to read the user password in memory and log in as the user, impersonate them, or make requests on their behalf.

**Business Impact**

This vulnerability can lead to reputational damage for the business due to a loss in confidence and trust by users.

**Steps to Reproduce**

1. Utilize some software that allows computer memory to be accessed in a human-readable format
1. Log in to the application
1. Navigate to the following URL: {{URL}} and perform {{action}}
1. Cease using the application
1. Using the computer memory viewer, view the password of the user that remained in memory after use

**Proof of Concept (PoC)**

The screenshot(s) below demonstrate(s) the vulnerability:
>
> {{screenshot}}
