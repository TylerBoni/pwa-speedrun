# 4. Supabase Dashboard

Free plan only includes 2 active projects, make sure you have a project available before starting presentation.
- https://supabase.com/dashboard/

## 1: Initial Setup 
- Create new project
- Set database password, save in PW manager

## 2: OAuth Setup
### Authentication → Sign In / Providers
- Enable Google Oauth
- Copy "Callback URL (for OAuth)"

### Go to google console -> Clients -> "Client Name"
- Authorized Redirect URIs -> Add Uri
- Paste Callback URL
- Save
- Copy Client ID, paste into supabase
- Copy Client Secret, paste into supabase
- Return to supabase and Configure Google OAuth provider credentials

### Back to Supabase
### Authentication -> URL Configuration
- Site URL (optional): use your url if you have one for Prod
- Redirect URLs -> Add URL
- Add "http://localhost:8080/**"
- Add production or testing URLs if you have them

# How OAuth works (Google = Provider, works the same for others)
- Supabase sends us to Google
- Google verifies our supabase application and scopes
- Google authenticates user
- Google sends Pass/Fail + user info to Supabase Redirect (#1)
- Supabase in browser redirects (#2) the user back to our application
- Browser stores temporary access token in browser cookies

