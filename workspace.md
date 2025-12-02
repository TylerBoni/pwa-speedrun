# Workspace Setup (1–9)

## 1. Presentation
- Slides (Google Slides / Keynote)
- Speaker notes
- Timer (optional)

## 2. Cloudflare Domain Registry
- Cloudflare dashboard
- Domain registration/transfer
- DNS configuration
- SSL/TLS settings

## 3. Supabase Dashboard
Free plan only includes 2 active projects, make sure you have a project available before starting presentation.
- https://supabase.com/dashboard/

### Phase 1: Initial Setup 
- Create new project
- Set database password: AWU^IqnXr8VtUN

### Phase 2: OAuth Setup (After Lovable)
- Authentication → Providers
- Configure Google OAuth provider
- Set redirect URLs

### Phase 3: Review (Towards End)
- Review project settings
- Verify connections
- Check Edge Functions tab

## 4. Lovable (PWA Build)
- https://lovable.dev (dashboard)
- Lovable project page
- Project Settings → Integrations → Supabase (connect using URL + anon key from Supabase Phase 1)
- Live preview (open in a NEW TAB)
- GitHub repo (Lovable-linked)

## 5. GitHub Repo
- GitHub project main page
- GitHub Actions for deployments
- Code viewer of src/ (e.g., src/pages, src/components)

## 6. Google Cloud Console (OAuth)
- https://console.cloud.google.com
- Google Auth Platform → Configure
- APIs & Services → OAuth consent screen
- APIs & Services → Credentials → OAuth Client
- Test Users page
- Data Access API settings

## 7. Local Code Editor
- VS Code / JetBrains with project open
- .env.local / .env.production
- supabase/functions/* folders
- tailwind.config, package.json, etc.

## 8. Terminal (Supabase CLI / Dev tools)
- supabase login
- supabase start (optional)
- supabase functions deploy <name>
- npm run dev
- git status / git push

## 9. Live App Preview
- Production URL
- Lovable preview URL
- DevTools → Application → Manifest
- Mobile device simulation enabled

## 10. Domains / Deployment / Misc
- Lovable → Deployments tab
- Supabase → Project Settings → Redirect URLs
- Reference docs:
  - Supabase CLI docs
  - Deno runtime docs
  - Google Auth Platform docs
