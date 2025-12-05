# 3. Google Cloud Console (OAuth Configuration)

## Overview
Configure OAuth 2.0 credentials in Google Cloud Console to enable authentication for your application.

**Access:** https://console.cloud.google.com

## Step 1: Create Project

1. Navigate to **New Project**
2. Enter your application name
3. Click **Create** and select the newly created project

## Step 2: Enable Google Authentication Platform

1. Use the search bar to locate **Google Authentication Platform**
2. Click **Get Started** to initialize the authentication service

## Step 3: Configure Application Information

### Application Details
- **Application Name:** Enter your application name

### Audience Selection
Choose the appropriate audience type for your use case:

- **Internal:** Restricted to users with email addresses from your domain (e.g., @yourdomain.com). Recommended for internal company tools and applications.
- **External (Recommended):** Suitable for public-facing applications. Note: Applications remain in testing mode until verified by Google.

## Step 4: Create OAuth 2.0 Client

1. Click **Create OAuth Client**
2. Configure the following settings:
   - **Application Type:** Web Application
   - **Name (Optional):** Enter a descriptive name (e.g., "Supabase Integration"). This name is not displayed to end users.
3. Click **Create**

## Step 5: Configure Supabase Integration

After creating the OAuth client, proceed to configure the integration in Supabase:

1. **Add Redirect URI:** Copy the authorized redirect URI from Supabase and add it to your OAuth client configuration
2. **Copy Client ID:** Retrieve the OAuth Client ID from Google Cloud Console
3. **Copy Client Secret:** Retrieve the OAuth Client Secret. If a secret is not visible, create a new one from the credentials management page
4. Enter these credentials in your Supabase project settings
