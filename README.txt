━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  📸 Instagram Stats Telegram Bot - SETUP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

STEP 1 — Get Bot Token
───────────────────────
1. Open Telegram → search @BotFather
2. Send /newbot
3. Give it a name and username
4. Copy the TOKEN it gives you

STEP 2 — Get Your Admin ID
───────────────────────────
1. Open Telegram → search @userinfobot
2. Send /start
3. Copy your numeric ID (e.g. 123456789)

STEP 3 — Create Your Channel
──────────────────────────────
1. Create a Telegram channel
2. Add your bot as Admin of the channel
3. Copy the channel username (e.g. @mychannel)

STEP 4 — Edit bot.py
──────────────────────
Open bot.py and fill these 4 lines at the top:

  BOT_TOKEN        = "PASTE_YOUR_BOT_TOKEN_HERE"
  ADMIN_ID         = 123456789        ← your numeric ID
  CHANNEL_USERNAME = "@your_channel"  ← your channel
  CHANNEL_LINK     = "https://t.me/your_channel"

STEP 5 — Install & Run
────────────────────────
# Install Python 3.10+ first if needed

pip install -r requirements.txt
python bot.py

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  BOT COMMANDS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

USER COMMANDS:
  /start              → Welcome + credit info
  /help               → How to use
  /credits            → Your credit balance
  /referral           → Your referral link
  /check username     → Check 1 account
  Just type usernames → Check up to 10 at once

ADMIN COMMANDS (only your ADMIN_ID can use):
  /admin              → Admin panel
  /stats              → Full bot statistics
  /users              → List all users
  /broadcast TEXT     → Send message to all users
  /addcredits ID AMT  → Add credits to a user
  /removecredits ID AMT → Remove credits

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  CREDIT SYSTEM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  🎁 New user joins         → 20 FREE credits
  📊 Check 1 IG account     → 1 credit used
  ⚡ Check up to 10 at once  → 10 credits max
  🔗 Someone uses your code  → +1 credit for you
  📩 You use someone's code  → +1 bonus credit

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  HOSTING (keep bot running 24/7)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Free options:
  • Railway.app     → railway.app (easy deploy)
  • Render.com      → render.com
  • Replit          → replit.com (always-on plan)

VPS (best):
  • Contabo VPS ~$5/mo
  • DigitalOcean Droplet
  • Use: screen python bot.py  (or systemd service)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  NOTE ON INSTAGRAM SCRAPING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

This bot uses "instaloader" to fetch public IG data.
  ✅ Works for public profiles
  ❌ Cannot access private profiles
  ⚠️  Instagram may rate-limit heavy usage
     → Add a delay between checks if needed

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
