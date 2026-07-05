# Jarvis AI Manager

**Production-ready AI automation platform for Sales, Operations & Production teams.**

## What It Does

✅ Chat interface with AI manager
✅ Send WhatsApp/Slack/Email automations
✅ Update CRM contacts in real-time  
✅ Generate sales & revenue reports
✅ Track team performance metrics
✅ All integrated, tested, production-ready

## Tech Stack

- **Frontend:** HTML/JS (no build process)
- **Backend:** Node.js + Express
- **Database:** PostgreSQL
- **Deployment:** Railway (or Render)

## Local Development

```bash
# Install
npm install

# Create .env
cp .env.example .env
# Edit .env with your DATABASE_URL

# Run
npm start

# Visit http://localhost:5000
```

## Deploy to Production

See **DEPLOY.md** for step-by-step instructions.

**TL;DR:**
1. Push to GitHub
2. Create PostgreSQL on Railway
3. Deploy app to Railway
4. Add DATABASE_URL variable
5. Done. Live in 5 minutes.

## API Endpoints

- `POST /api/chat` - Send message to Jarvis
- `POST /api/automation/whatsapp` - Send WhatsApp
- `POST /api/automation/crm` - Update CRM
- `POST /api/automation/slack` - Post to Slack
- `POST /api/automation/email` - Send email
- `GET /api/messages` - Chat history
- `GET /api/automations` - Automation history

## Client Access

After deployment, share the public URL with your client.
They can immediately start using it - no setup needed.

## Customization

Edit code, push to GitHub, Railway auto-deploys.

```bash
git add .
git commit -m "Update"
git push
```

Updates live in 2 minutes.

---

**Built for production. Ready to deliver.**
