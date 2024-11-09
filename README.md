
# 🥥 Coconuts for Padded Helmets 🥥

![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)
![Build Status](https://img.shields.io/github/actions/workflow/status/nerdboy1024/coconuts-for-padded-helmets/build.yml)
![Hosted on Railway](https://img.shields.io/badge/hosted%20on-Railway-blueviolet)

**Coconuts for Padded Helmets** is a Discord bot aimed at playfully handling users who ask questions just to get attention. 
Think of it as your server’s very own sarcastic nanny, here to keep the chaos in check and hand out padded helmets when needed. 🥳

## Features

- 🚨 **Detects Attention-Seeking Questions**: The bot has a sixth sense for spotting users fishing for attention – no bait needed.
- 🤖 **Sassy Replies**: Expect snarky comebacks and cheeky responses that make everyone laugh (except the attention seeker).
- 📝 **Tracking System**: Keeps score of attention-seeking behavior like a referee in a game nobody wants to win.
- 🎭 **Customizable Responses**: Want the bot to call out your friends in style? Customize the responses for maximum effect.
- 🧑‍💬 **Optional Special User Replies**: Automatically replies to Coconuts (because we all know he’ll be testing the bot nonstop). This feature can be toggled off if the server needs a break.
- 🔨 **Optional Moderation**: Give the bot a little authority, and it will start issuing warnings, mutes, and even kicks faster than you can say “calm down.”

## Additional Features

- 🏆 **Attention Seeker Leaderboard**: Keep track of who’s leading the race to the padded helmet.
- ⏳ **Cooldown Mechanism**: Built-in cooldowns because even Coconuts needs to take a breath once in a while.
- 🎨 **Customizable Responses**: Make the bot sound like Shakespeare or your grumpy uncle – it’s up to you!
- 📊 **Statistics Command** (`!stats`): Want to see how many times the bot’s called out Coconuts? Check the stats for a laugh.
- 🎮 **Minigames**: Distract attention-seekers with a game of “Guess the Emoji” or a quick quiz.
- 🎉 **Event-Based Replies**: The bot can even roast Coconuts when he joins a voice channel – it’s like a welcoming committee with attitude.
- 🔧 **Dynamic Response Frequency**: Adjust how often the bot replies – from “Chill Mode” to “Relentless Sarcasm.”
- 🥥 **Attention-Seeker Role Assignment**: Earn the prestigious title of “Resident Coconut” for repeated offenses.
- 📈 **Logging and Analytics**: Detailed logs of all the hilarity for admins to review (and laugh at).
- 🤝 **Friendly Reminder Mode**: The bot can gently guide users who seem lost or confused, with a smile and a wink.

## Configuration File

The bot includes a configuration file (`config.json`), allowing admins to:
- Enable/disable special user replies.
- Adjust response sensitivity (from gentle nudges to full-on sarcasm).
- Toggle moderation features (warnings, mutes, and kicks).

## Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com/).
2. Create a new project and download `firebase_credentials.json`.
3. Add the path to `.env`:
   ```
   FIREBASE_CREDENTIALS=firebase_credentials.json
   ```

## Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/nerdboy1024/coconuts-for-padded-helmets.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure your `.env` file with your bot token and Firebase credentials.
4. Start the bot:
   ```bash
   python bot.py
   ```

## Invite the Bot

Invite the bot with this link (don’t forget the padded helmet for protection):
```
https://discord.com/oauth2/authorize?client_id=YOUR_CLIENT_ID&permissions=8&scope=bot
```

## Support and Contact

Need help? Encounter a bug (or did Coconuts break it again)? Reach out via:
- GitHub Issues: [Report an Issue](https://github.com/nerdboy1024/coconuts-for-padded-helmets/issues)
- Discord Support Server: (Link Coming Soon)

## Contributors

A huge thank you to everyone brave enough to contribute to this project! If you’d like to join the fun (or chaos), submit a pull request.

## Security and Privacy Notice

The bot uses Firebase to store user interaction data. Don’t worry – no sensitive personal data is collected, just logs of Coconuts’ antics for everyone’s amusement.

## FAQ

- **Q: The bot isn’t replying to Coconuts. What’s wrong?**
  - A: Did Coconuts change his username again? Check the config file before he breaks something else.

- **Q: The bot keeps responding to every message. How do I stop it?**
  - A: Adjust the sensitivity settings, or give the bot a coffee break.

- **Q: Firebase isn’t connecting. Help!**
  - A: Check your `firebase_credentials.json` and `.env` setup. Did Coconuts accidentally delete the credentials file?

## Roadmap

- 🛠️ **Enhanced User Tracking**: More detailed analytics for attention-seeking patterns.
- 🗣️ **Voice Channel Integration**: Roast Coconuts as soon as he joins a voice chat.
- 📈 **Statistics Dashboard**: A web dashboard to showcase the bot’s interactions and Coconuts’ leaderboard position.
- 🧩 **Plugin System**: For even more chaotic features.

## Code of Conduct

Be kind and patient, especially when dealing with Coconuts. Remember, this bot exists to make us all laugh (and maybe cringe a little).

## License

This project is licensed under the MIT License.


## Project Structure

Here’s how the project is organized, so you can easily find your way around:

```
coconuts-for-padded-helmets/
├── .env.example          # Example environment variables file
├── README.md             # Project README with all details
├── requirements.txt      # Python dependencies
├── config.json           # Configuration file for bot settings
├── firebase_credentials.json (not uploaded) # Firebase credentials (add to .gitignore)
├── bot.py                # Main bot script
├── utils/
│   ├── __init__.py       # Init file for utils package
│   └── firebase.py       # Firebase setup and helper functions
├── commands/
│   ├── __init__.py       # Init file for commands package
│   ├── moderation.py     # Moderation commands and features
│   └── responses.py      # Custom responses and special user replies
├── .gitignore            # Ignore sensitive files and cache
├── .github/
│   └── workflows/
│       └── build.yml     # GitHub Actions workflow for CI/CD
```

### Key Files:

- **`.env.example`**: Example file with placeholders for environment variables (bot token, Firebase path).
- **`requirements.txt`**: Specifies Python dependencies.
- **`config.json`**: Configuration options for bot behavior (e.g., moderation enabled, special user replies).
- **`firebase_credentials.json`**: Firebase credentials (not uploaded, should be listed in `.gitignore`).
- **`bot.py`**: Main script to run the bot.
- **`utils/firebase.py`**: Helper functions for interacting with Firebase.
- **`commands/`**: Contains all bot commands (e.g., moderation, responses).
- **`.gitignore`**: Excludes sensitive files from being pushed to GitHub.
- **`build.yml`**: GitHub Actions configuration for automatic builds and testing.

This structure helps keep the project organized and easy to maintain. 🛠️

