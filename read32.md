# Reading 11
1-What is OAuth?
OAuth: open protocol/framework allow authenticated access without credentials.
2-Give an example of what using OAuth would look like: 
an example is when we use Netlify or Herouku and it authintacte us directly from our github accounts. 

3-How does OAuth work? What are the steps that it takes to authenticate the user?
The user initiates a transaction to access another site. 
The steps as mentiond in the article : 
"The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
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
OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons)."
4-What is OpenID?
another security technology but its authentication not authorization as OAuth.
or as said "OpenID is for humans logging into machines"
it seves as a single sign in. 


What is the difference between authorization and authentication?
Authentication means confirming your own identity, while authorization means granting access to the system
What is Authorization Code Flow?
exchanges an Authorization Code for a token
What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
Additional security.
What is Implicit Flow with Form Post?
it helps Public Clients/ applications to securely store Client Secrets.
What is Client Credentials Flow?
machine-to-machine is where the system authenticates and authorizes the app instead of you as a user. 

What is Device Authorization Flow?
Input-constrained devices that connect to the internet through a link. 

What is Resource Owner Password Flow? 
An interactive form where the user us providing username and password. 