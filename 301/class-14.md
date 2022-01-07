# Class 14 Reading Notes

---

## Things I want to know more about

- How we implement Auth0 in our apps.

---  
## What is OAuth

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

### Question Answers: 

*What is OAuth?*

"OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization."

*Give an example of what using OAuth would look like.*

When you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. 

*How does OAuth work? What are the steps that it takes to authenticate the user?*
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. he client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.

*What is OpenID?*
-  First a competitor of, now an authentication layer for OAuth. It was a technology for allowing a user to have one log in for multiple sites, rather than logging into one site and having that site log into another for you. 

---

## Authorization and Authentication flows

- [Authorization and Authentication flows](https://auth0.com/docs/authorization/flows)

### Question Answers: 

*What is the difference between authorization and authentication?*
    - Authentication proves who someone is, authorization proves that someone is allowed to do something (access resources, etc...).

*What is Authorization Code Flow?*
    - Used for regular web apps, it provides the clients secret token with the server, the server then authorizes the request and responds.

*What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?*
    - For mobile apps (native and single page), like Auth code flow, but must generate an additional challenge on the client side, which is then solved on the server side. This is because these apps cannot protect a clients secret token.

*What is Implicit Flow with Form Post?*
  -  The web app requests and obtains tokens through the front end, without the need for secrets or extra backend calls. Use for login only. 

*What is Client Credentials Flow?*
- A machine to machine authorization flow.

*What is Device Authorization Flow?*
- An authorization flow that allows a device to be authorized, rather than a user.

*What is Resource Owner Password Flow?*
- Not recommended, a user can log in through an interactive form, then that username and password are stored server side. Should only be used in a completely trusted system, and even then probably not. 