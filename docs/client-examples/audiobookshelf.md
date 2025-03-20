---
id: audiobookshelf
---
# Audiobookshelf

## Pocket ID Setup

1. In Pocket ID, create a new OIDC client named `Audiobookshelf` (or any name you prefer).  
2. (Optional) Set a logo for the OIDC client.  
3. Set the callback URLs to:
`https://<your.server.com>/auth/openid/callback` and
`https://<your.server.com>/auth/openid/mobile-redirect`
4. Set the logout callback URL to:
`https://<your.server.com>/application/o/audiobookshelf/end-session/`
5. Copy the `Client ID`, `Client Secret`, and `OIDC Discovery URL` for the next steps.  

## Audiobookshelf Setup

1. Log in to Audiobookshelf as an admin.  
2. Go to **Settings → Authentication**.  
3. Check **OpenID Connect Authentication**.  
4. Enter the `OIDC Discovery URL` into the **Issuer URL** field then click **Auto-populate**. 
5. Enter the `Client ID` into the **Client ID** field.  
6. Enter the `Client Secret` into the **Client Secret** field.  
7. Enter the `Client ID` into the **Client ID** field.  
8. Enter the `Client Secret` into the **Client Secret** field.  
9. Save the settings and test the OAuth login.  
