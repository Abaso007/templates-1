Stored Cross-Site Scripting (XSS) is a type of injection attack where malicious JavaScript is injected into a website. When a user visits the affected web page, the JavaScript executes within that user’s browser in the context of this domain. Stored XSS can be found on this domain which allows an attacker to submit data to a form and escalate from no privileges to any user type, which could include an Administrator level user.

When an attacker can control code that is executed within a user’s browser, they are able to carry out any actions that the user is able to perform, including accessing any of the user's data and modifying information within the user’s permissions. This can result in modification, deletion, or theft of data, including accessing or deleting files, or stealing session cookies which an attacker could use to hijack a user’s session.

to create a crafted JavaScript payload. When a user navigates to the page,  the arbitrary JavaScript executes within that user’s browser in the context of this domain.

**Business Impact**

Stored XSS could lead to data theft through the attacker’s ability to manipulate data through their access to the application, and their ability to interact with other users, including performing other malicious attacks, which would appear to originate from a legitimate user. These malicious actions could also result in reputational damage for the business through the impact to customers’ trust.

**Steps to Reproduce**

1. Enable a HTTP interception proxy, such as Burp Suite or OWASP ZAP
1. Navigate to {{URL}}
1. Forward the following request to the endpoint:

```HTTP
{{request}}
```

1. Log in to a privileged account (User A) and navigate to {{url}} which contains the payload
1. Observe the JavaScript payload being executed, capturing the cookies of User A
1. Log out of User A’s account

**Proof of Concept (PoC)**

The screenshot(s) below demonstrate(s) the vulnerability:
>
> {{screenshot}}
