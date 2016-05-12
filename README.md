# Disable HTTP in Tomcat

This is an example that shows how to forward all HTTP requests in Tomcat to the same URL with the HTTPS protocol.

On Heroku, this is the prefered way of disabling HTTP because the Heroku router is responible for terminating the
SSL, and thus Tomcat doesn't use a `server.xml` to configure HTTPS.