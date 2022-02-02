# 401 - Class 07 Reading Notes

---

## REVIEW, RESEARCH, DISCUSSION

1. Write the following steps in the correct order:
  - Register your application to get a client_id and client_secret
  - Receive access token
  - Receive authorization code
  - Ask the client if they want to sign in via a third party
  - Redirect to a third party authentication endpoint
  - Make a request to the access token endpoint
  - Make a request to a third-party API endpoint


What can you do with an authorization code?
  -  validates a person's identity
What can you do with an access token?
  - Access tokens are used in token-based authentication to allow an application to access an API. 
What’s a benefit of using OAuth instead of your own basic authentication?
  - You have an industry recognized authentication system made by an entire team/company, and the years of work/know-how that went into building it when using OAuth.

--- 

## Vocabulary Terms

  - Client ID: a public identifier for apps. 
  - Client Secret: a secret known only to the application and the authorization server.
  - Authentication Endpoint: a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.
  - Access Token Endpoint: is used by the application in order to get an access token or a refresh token. 
  - API Endpoint: An API endpoint is a digital location where an API receives requests about a specific resource on its server.
  - Authorization Code: is a temporary code that the client will exchange for an access token. 
  - Access Token: used in token-based authentication to allow an application to access an API. 

--- 

## Resources 

RESOURCES: [Auth0 Docs](https://auth0.com/docs)
RESOURCES: [OAuth 2.0 Simplified](https://www.oauth.com/)
