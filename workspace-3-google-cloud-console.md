# 3. Google Cloud Console (OAuth)

- https://console.cloud.google.com
- New Project -> Your App
- Select Project
- Search -> Google Auth Platform → Get Started
- App Info:
    - Your App Name
    - Audience:
        - Internal - Only users with @yourdomain.com
        - External - Only for testing until app is verified
- Create OAuth Client
    - Type: Web Application
    - Name (optional): Supabase - not shown to end users
    - #### Redirect URI: This will come from supabase on the next page.
- Data Access (optional)
    - These are the scopes that you want to use. For example, if you wanted to build an application that sent emails for the user, you could use the Gmail API in this tab.

### Phase 2 - Supabase
- Add Redirect URI
- Copy Client ID
- Copy Client Secret (if not available create a new secret)
