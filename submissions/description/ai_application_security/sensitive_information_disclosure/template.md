Personal Identifiable Information (PII) disclosure occurs when an AI system unintentionally exposes PII. An attacker can abuse flaws in the system's isolation mechanisms or errors in data handling and processing to access sensitive data intended for a specific user or organization.

**Business Impact**

This vulnerability can lead to reputational and financial damage of the company due an attacker gaining access to unauthorized data, which would also impact customers' trust. The severity of the impact to the business is dependent on the sensitivity of the accessible data being transmitted by the application.

**Steps to Reproduce**

1. Log in to the AI system with credentials for Tenant A
1. Send the following request targeting the PII data or resources:

``` HTTP
  {HTTP request}
```

1. Observe that PII is disclosed

**Proof of Concept (PoC)**

The screenshot(s) below demonstrate(s) the vulnerability:
>
> {{screenshot}}
