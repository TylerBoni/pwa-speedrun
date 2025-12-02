# 5. Lovable (PWA Build)

## Connect to Supabase:
- "+" icon on prompt -> Integrations

## Themes and images
- Attach photos and/or use "Theme" before sending prompt for better styling results: https://heycolab.com

## Prompt
- Use chatgpt or similar to generate a prompt to save on tokens.
- The prompt below has been simplified as much as possible so it can be used by only changing the upper section
- Recommend using chatgpt to generate table schemas and expand this prompt for better results.
Prompt for demonstration:
```
###########
Name: CoLab Now

Domain: colab.tylerboni.com

Problem: At my coworking space (CoLab Coworking), we play music with Spotify.
I am the manager and there is no way to tell if people like or dislike songs.

Goal: Create an app that members can Like, dislike, comment, request songs that are currently playing.

Challenges: Making sure only active members can participate. Some members may want to stay anonymous when participating

Audience: Members of CoLab, and Staff (admins) of CoLab

Future considerations: In the future I may add other systems that are not related to music.

Style: Light theme. Simple and clean, prioritizing using logos instead of text labels.
Design with Apple's mentality of clean, simple, and intuitive interfaces.
Prioritize mobile development. 
Our colors are white, dark grey, and teal

External Services: Spotify API

###########

Build a React SPA (PWA) with Radix UI, Tailwind, and Supabase (Auth, PostgREST, Storage).

🔧 Tech

Framework: React SPA (Vite) + Capacitor for iOS and Android build

UI: Radix (Tabs, Dialog, Sheet, Toast, Avatar, Progress, Dropdown)

Styling: Tailwind (minimal custom components)

State: TanStack Query

Auth: Supabase OAuth (Google)

API: Supabase PostgREST (no custom backend)

Storage: Supabase Bucket Storage 

DB: Supabase postgres

PWA: manifest, service worker, offline page

Vercel: Include a minimal vercel.json to avoid path errors:
{
    "rewrites": [{ 
        "source": "/(.*)",
        "destination": "/" }]
}

🔐 Auth + Roles

Providers: Google, Microsoft

Redirect (dev): http://localhost:8080/auth/callback

Roles: admin, user

💅 UI Components

Use Radix + Tailwind for: Header, Tabs, Dialogs, Progress, Toasts. 

Key UI: AccountCards, SignInDialog. 

Hooks: useQueryTab(), useAuth()

🔌 Data Access 
PostgREST via Supabase client

🧭 Logic
OAuth redirect preserves returnTo

📱 PWA
Files: /manifest.webmanifest, /service-worker.js, /offline

🧩 Acceptance
Tabs switch via ?tab= (no full reload)

Auth via Supabase works (OAuth + redirect)

PWA installable + offline fallback

Cache data with indexeddb to improve performance and offline ability

🧪 Mock Seed
Migrations are in /supabase/migrations
Create 5 items for every table necessary to seed in a separate migration SQL file called "seed.sql", as well as a seed function to fill indexdb with cache data if env is NOT production


Build the full project with this structure, using Supabase PostgREST for all CRUD, Radix for UI, Tailwind for styling, and React Query for data. Keep everything tenant-aware and offline-ready.
```

## Preview
- OAuth doesn't work well in the preview pane
- "Open Preview In New Tab" button is the diagonal arrow next to the refresh button in the preview menu bar on top
- Do not use lovable to add functionality UNLESS it is visual
- Check mobile views while here
- Check console logs for errors

## Security Scan
- Pay attention to it, but do not use lovable to fix it
- Fix with cursor in next phase

## Connect to Github
- When ready to move to next phase, connect to github
- 2 way sync: Lovable will push to main branch, and also pull automatically
- You can leave lovable, make changes manually in cursor, push to main and return to lovable
- If you make changes in lovable after local development, you need to pull these changes in your local environment
- recommend creating dev and prod branches