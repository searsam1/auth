Cookie Security
Cookies often store sensitive information, especially when they’re used in session management. Cookies are also used to store a user’s personal preferences or history, which should also stay secure.

It’s important to add security to the cookies, especially in the case that someone tries to swipe data from them to steal your session data!

The first step to securing a cookie could be adding an expiration date or duration so a cookie doesn’t persist longer than it needs to. We can specify that information through the Set-Cookie header in an HTTP response like so:

Set-Cookie: Key=Value; expires=Saturday, 01-May-2021 07:30:10 GMT

The HttpOnly attribute for the Set-Cookie header makes sure that the cookie’s data is not accessible to a script running client-side. This helps prevent a Cross-Site Scripting (XSS) attack that tries to steal a session cookie and take over the victim’s session, which is extremely common.

Set-Cookie: Key=Value; expires=Saturday, 01-May-2021 07:30:10 GMT; HTTPOnly

Here are some other Set-Cookie options:

SameSite helps prevent Cross-Site Request Forgery (CSRF) attacks.
Secure makes sure cookies are only sent with a request to an HTTPS page.