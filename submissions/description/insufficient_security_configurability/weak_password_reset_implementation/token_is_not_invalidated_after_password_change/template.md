The password reset implementation needs to involve a unique, temporary high-entropy token that has a short expiry and can only be used once. When these conditions are not met, the password reset implementation is  considered weak. This diminishes the strength of the overall authentication process for the application and can lead to account takeover.

The application does not invalidate the password reset token after a password change. If an attacker were to gain access to the system used to store the reset token, they could use this unused token to reset the user's password and gain access to the account.

**Business Impact**

Weak password reset implementation can result in reputational damage for the business through the impact to customers’ trust as they could believe that the business doesn’t take their account security seriously or trust that their data within will remain secure.

If an attacker successfully takes over an account by capturing a password reset token, it can lead to data theft from the business. The severity of the impact to the business is dependent on the sensitivity of the data being stored in, and transmitted by the application, as well as the level of access gained by an attacker.

**Steps to Reproduce**

1. Use a browser to log in and navigate to: {{URL}}
1. Initiate a password reset
1. Modify the password for the account
1. Observe that the password reset token received earlier is still valid

**Proof of Concept (PoC)**

The following screenshot shows that the password reset token is not invalidated after a password change:

{{screenshot}}
