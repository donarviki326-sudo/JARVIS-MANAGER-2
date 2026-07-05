# DEPLOY TO RAILWAY (5 MINUTES)

## Prerequisites
- GitHub account
- Railway account (free)

## Step 1: Push to GitHub

```bash
git init
git add .
git commit -m "Jarvis Manager - Ready to deploy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/jarvis-manager.git
git push -u origin main
```

## Step 2: Create PostgreSQL on Railway

1. Go to https://railway.app
2. Click **"New Project"** → **"Provision PostgreSQL"**
3. Wait for database to initialize
4. Click the PostgreSQL card
5. Go to **"Connect"** tab
6. Copy the **PostgreSQL connection string** (looks like: `postgresql://user:pass@host:port/db`)

## Step 3: Deploy App to Railway

1. Go back to Railway dashboard
2. Click **"New"** → **"GitHub Repo"**
3. Connect your GitHub account
4. Select: `YOUR_USERNAME/jarvis-manager`
5. Railway auto-detects it's Node.js
6. Click **"Deploy"**

## Step 4: Add Database URL

In Railway dashboard:
1. Click your **jarvis-manager** project
2. Click **"Variables"**
3. Add new variable:
   - Name: `DATABASE_URL`
   - Value: (paste the PostgreSQL connection string from Step 2)
4. Click **"Save"**

## Step 5: It's Live!

Railway shows your public URL like:
```
https://jarvis-manager-prod.up.railway.app
```

Your client visits that URL and starts using it immediately.

---

## What's Included

✅ Chat UI - Beautiful, responsive
✅ Backend API - Express.js  
✅ Database - PostgreSQL
✅ Automations - WhatsApp, CRM, Slack, Email
✅ Reports - Revenue, Pipeline, Team Performance
✅ All integrated and tested

---

## For Client Access

Send your client the Railway URL:
```
https://jarvis-manager-prod.up.railway.app
```

They can immediately:
- Chat with Jarvis AI Manager
- Send WhatsApp/Slack/Email automations
- View team reports
- Update CRM contacts

No setup needed on their end.

---

## Customization (After Deployment)

Edit anything in the code, push to GitHub, Railway auto-deploys:
```bash
git add .
git commit -m "Update features"
git push
```

Done. Updates live in 2 minutes.

---

## Support

- Database issues? Check Railway's PostgreSQL logs
- API errors? Check Railway's app logs
- Need to scale? Railway handles it automatically
