VORTEX BOT - RENDER SETUP

1. Keep these files in the ROOT of your GitHub repository:
   - requirements.txt
   - runtime.txt
   - render.yaml
   - vortexBot.py

2. Rename your bot script to exactly:
   vortexBot.py

3. In Render, create a Background Worker from this repository.
   The render.yaml config uses:
   Build: pip install -r requirements.txt
   Start: python vortexBot.py

4. IMPORTANT:
   - These setup files fix the missing requirements.txt issue and select Python 3.12.
   - They cannot guarantee that the bot code itself has no errors.
   - The bot token/API credentials previously included in the uploaded source should be treated as exposed.
     Revoke/regenerate the bot token in BotFather, then store credentials as Render environment variables.
   - Do not commit bot tokens, API hashes, or other secrets to a public GitHub repository.
