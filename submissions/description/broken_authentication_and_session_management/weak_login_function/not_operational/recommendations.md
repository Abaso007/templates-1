# Recommendation(s)

Weak login function can be remediated by implementing a handful of best practices relating to authentication and session management to ensure secure implementation. These include:

- Removing or restricting public access to endpoints that are not operational
- If the endpoint is intended for public access, consider using multi-factor authentication (MFA), to reduce the risk of unauthorized access
- Enabling HTTPS for the login page and all subsequent authenticated pages
- Disable the option of forcing a HTTP connection by browsers
- Implement the HTTP Strict Transport Security (HSTS) header
- Keeping all systems, software and operating systems up-to-date with a repeatable patch management process
- Validate all user input server-side
- Ensure that the authentication mechanisms and logic are robust and that each request for a resource passes through an authorization process

The verification logic of the application, as well as all of the above, should be thoroughly tested during the development and QA phases of an application build.

For further information, refer to Open Web Application Security Project(OWASP) guides located at:

- <https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html#transmit-passwords-only-over-tls-or-other-strong-transport>
- <https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html>
- <https://owasp.org/Top10/A07_2021-Identification_and_Authentication_Failures/>
