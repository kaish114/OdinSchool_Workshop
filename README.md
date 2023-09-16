# OdinSchool_Workshop

# Telegram AI Bot

This is a Telegram bot that can respond to user messages using AI from OpenAI model.

## Overview

The bot uses the Python Telegram Bot API wrapper and either the OpenAI API or Anthropic's G4F library to generate responses to user messages.

Key features:

- Responds to the `/start` command with a greeting message
- Handles text messages from users and generates a response using OpenAI or GPT-3.5
- Asynchronously generates GPT-3.5 responses using a thread pool executor 
- Loads API keys and tokens from environment variables for security

## Setup

1. Sign up for an [OpenAI](https://openai.com/) API key.

2. Save the API keys in a `.env` file:

```
OPENAI_KEY=sk-...
TG_BOT_TOKEN=123456:ABC...
```

3. Install requirements:

```
pip install python-telegram-bot python-dotenv openai g4f
```

4. Run `python telegram_bot.py` to start the bot.

5. Message your bot and interact!

## Customizing

- Switch between using OpenAI and GPT-3.5 by commenting/uncommenting code and API keys.
- Modify `echo()` handler to call different AI models.
- Add new command handlers for additional bot features.

## Resources

- [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot)
- [OpenAI API](https://openai.com/api/)
- [GPT-3.5 API](https://www.anthropic.com/)
