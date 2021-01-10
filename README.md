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
1/8/2021 - Learning about SSO - There is single-sign on and seamless sign-on. Both have identical end user
           experience but operate differently. Same sign-on is a different experience in which the same pw
           will work across services but all of them individually prompt for the password
1/9/2021 - Learned a lot of loose ends. Dove into enabling different methods of MFA and passwordless authentication.
           Focused on something you know, have, and are. Also dove deeper into conditional access and how VPN can play
           into that as well.
