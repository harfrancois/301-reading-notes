# What is OAuth

source: https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

#### What is OAuth?

An authentication service

#### Give an example of what using OAuth would look like.

Logging in to your email account.

#### How does OAuth work? What are the steps that it takes to authenticate the user?

When trying to understand OAuth, it can be helpful to remember that OAuth scenarios almost always represent two unrelated sites or services trying to accomplish something on behalf of users or their software. All three have to work together involving multiple approvals for the completed transaction to get authorized.

#### What is OpenID?

OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

# Authorization and Authentication flows

source:https://auth0.com/docs/get-started/authentication-and-authorization-flow

#### What is the difference between authorization and authentication?

Authorization is making sure your allowed to access what your trying to access. Authentication is making sure the persons identity matches. 

#### What is Authorization Code Flow?

Authorization Code Flow, which exchanges an Authorization Code for a token.

#### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

#### What is Implicit Flow with Form Post?

As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.

#### What is Client Credentials Flow?

With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4).

#### What is Device Authorization Flow?

With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.

#### What is Resource Owner Password Flow?

Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.

