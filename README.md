# AzPlayground
Playground for azure

## Initial plan for authentication

With basic Angular app scaffolded, authentication will be put in place as follows:

* Create OAuth page in Azure for Auth Code + PKCE
* Support Azure AD as IDP for admins
* Support Azure AD B2C for consumer authentication via appropved IDPs (Azure AD, Google, etc.)
* Learned about AD Connect,  which we will skip for now - no on premise AD to connect with
* Will focus entirely on cloud only auth first, then work in federation somehow

## Initial plan for authorization

* Create groups/roles with AAD

## Learning Log

1/6/2021 - Played around in Azure with tenants, subscriptions, resource groups, etc.
1/7/2021 - Dove into methods of authentication with AD Connect - Federation and Pass-Through
           Pass-Through will take the u/p and pass them onto AD while optionally storing pw hash in azure ad
           Federation - u/p skips Azure and goes straight to AD
