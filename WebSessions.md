SESSIONS & COOKIES VS. LOCALSTORAGE
Web Sessions
HTTP(S) protocol on its own is stateless, meaning requests and responses are just relaying information back and forth with no knowledge of a specific user.

But web developers want to create engaging, personalized experiences for users. This means there needs to be a system that associates the requests with a specific user and does so in a secure way. This is where sessions come in!

A web session refers to a series of user interactions over a time frame. Session data is stored server-side and associated with a session ID.

Think of a session as short-term memory for a web application. In the next exercise, we will explain where this session identifier is kept so that the browser (client) can keep retrieving the same session data between different page loads.