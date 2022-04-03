# Class15 Reading Notes

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

What is OAuth? is an open-standard authorization protocol or framework
Give an example of what using OAuth would look like. 
when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon
How does OAuth work? What are the steps that it takes to authenticate the user?
he first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
The user approves (or their software silently approves) a particular transaction type at the first website.
The user is given an approved access token (notice it’s no longer a request token).
The user gives the approved access token to the first website.
The first website gives the access token to the second website as proof of authentication on behalf of the user.
The second website lets the first website access their site on behalf of the user.
The user sees a successfully completed transaction occurring.
OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

What is OpenID?

OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans

[Authorization and Authentication flows](https://auth0.com/docs/flows)

What is the difference between authorization and authentication? 

The user clicks Login within the regular web application.

Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint).

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.

Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.

Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret.

Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.

Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

Your application can use the Access Token to call an API to access information about the user.

The API responds with requested data.

What is Authorization Code Flow?

The user clicks Login within the application.

Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/token endpoint).

Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

Your application can use the Access Token to call an API to access information about the user.

The API responds with requested data.


What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

The user clicks Login within the application.

Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/token endpoint).

Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

Your application can use the Access Token to call an API to access information about the user.

The API responds with requested data.

What is Implicit Flow with Form Post?

The user clicks Login in the app.

Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

Your Auth0 Authorization Server redirects the user back to the app with an ID Token.

What is Client Credentials Flow?

Your app authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (/oauth/token endpoint).

Your Auth0 Authorization Server validates the Client ID and Client Secret.

Your Auth0 Authorization Server responds with an Access Token.

Your application can use the Access Token to call an API on behalf of itself.

The API responds with requested data.

What is Device Authorization Flow?

The user starts the app on the device.

The device app requests authorization from the Auth0 Authorization Server using its Client ID (/oauth/device/code endpoint).

The Auth0 Authorization Server responds with a device_code, user_code, verification_uri, verification_uri_complete expires_in (lifetime in seconds for device_code and user_code), and polling interval.

The device app asks the user to activate using their computer or smartphone. The app may accomplish this by:

asking the user to visit the verification_uri and enter the user_code after displaying these values on-screen

asking the user to interact with either a QR Code or shortened URL with embedded user code generated from the verification_uri_complete

directly navigating to the verification page with embedded user code using verification_uri_complete, if running natively on a browser-based device

The device app begins polling your Auth0 Authorization Server for an Access Token (/oauth/token endpoint) using the time period specified by interval and counting from receipt of the last polling request's response. The device app continues polling until either the user completes the browser flow path or the user code expires.

When the user successfully completes the browser flow path, your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token). The device app should now forget its device_code because it will expire.

Your device app can use the Access Token to call an API to access information about the user.

The API responds with requested data.

What is Resource Owner Password Flow?

he user clicks Login within the application and enters their credentials.

Your application forwards the user's credentials to your Auth0 Authorization Server (/oauth/token endpoint).

Your Auth0 Authorization Server validates the credentials.

Your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token).

Your application can use the Access Token to call an API to access information about the user.

The API responds with requested data.

## Bookmark/Skim
[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)

----
## Things I want to know more about


---
### [Home](https://github.com/MISalz/301_Reading_Notes)