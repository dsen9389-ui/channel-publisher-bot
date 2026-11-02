AUTOMATED CHANNEL SUBMISSION PUBLISHER

OVERVIEW
This Telegram bot allows users to submit content for review. Designated administrators receive moderation alerts with interactive inline buttons. Once approved, the post is automatically published to the configured target channel.

FEATURES
- Interactive step by step post submission form
- Moderator review queue with inline approval buttons
- Automatic posting to designated channels upon review approval
- SQLite tracking of submission statuses

LOCAL SETUP
1. Clone the repository
2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate
3. Install dependencies:
   pip install -r requirements.txt
4. Copy env file and set your variables:
   cp .env.example .env
5. Run the bot:
   python main.py

CLOUD DEPLOYMENT GUIDE (KOYEB / RENDER)
1. Create a repository on GitHub and push the code.
2. Sign up at Render or Koyeb.
3. Create a new Web Service or Background Worker.
4. Set environment variables: BOT_TOKEN, ADMIN_ID, TARGET_CHANNEL.
5. Select Python runtime and set build command to: pip install -r requirements.txt
6. Set start command to: python main.py
7. Deploy service.
