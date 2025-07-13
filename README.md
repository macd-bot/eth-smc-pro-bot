# ETH SMC Pro Bot

## Description
This is a lightweight Python Flask app that receives webhook signals (e.g. from TradingView) and sends alerts to Telegram. You can integrate your own logic with Delta Exchange or Binance here.

## Files
- `main.py` – Flask server with /webhook and /healthz
- `requirements.txt` – Required Python libraries
- `Procfile` – Used by Render to launch Gunicorn
- `.env.sample` – Template for environment variables

## Setup
1. Clone repo or upload to GitHub
2. Add environment variables in Render:
    - BOT_TOKEN (from Telegram)
    - CHAT_ID (your Telegram chat ID)
3. Deploy on Render (Free tier works)
4. Use /webhook for TradingView alerts

## Health Check
Access `https://your-app.onrender.com/healthz` to confirm it's running.