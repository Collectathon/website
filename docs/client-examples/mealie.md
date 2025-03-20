---
id: mealie
---
# Mealie

## Pocket ID Setup

1. In Pocket ID, create a new OIDC client named `Mealie` (or any name you prefer).  
2. (Optional) Set a logo for the OIDC client.  
3. Set the callback URLs to:
`https://<your.server.com>/login` and
`https://<your.server.com>/login?direct=1`
4. Enable **PKCE**
5. Copy the `Client ID`, `Client Secret`, and `OIDC Discovery URL` for the next steps.  

## Audiobookshelf Setup

1. Open your `.env` file from your Hoarder compose and add these lines:

```ini
  OIDC_AUTH_ENABLED = true
  OIDC_CONFIGURATION_URL = https://<your.pocket-id.com>/.well-known/openid-configuration
  OIDC_CLIENT_ID = <client id from the created OIDC client>
  OIDC_CLIENT_SECRET = <client secret from the created OIDC client>
  OIDC_PROVIDER_NAME = Pocket-ID (or name you prefer)
  OIDC_ADMIN_GROUP = <admin group name>
  OIDC_USER_GROUP = <user group name>
  OIDC_REMEMBER_ME = true | false
```
2. Save the settings and test the OAuth login.  
