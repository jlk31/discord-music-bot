# Discord Music Bot

This repository contains my code for a small personal project to learn how to use the discord.py and asyncio library in preparation for a piece of year 1 coursework on Discord Bot programming at **Northumbria University**

## Features

- Allows the user to enter a slash command in a discord channel
- The slash command contains '/play' and the desired song name
- The bot creates a query to search for the song on YouTube
- Once the song has been found, it will either be downloaded or streamed
- The bot will join the same voice channel as the user who typed the command
- When in the voice channel, the requested song will start playing if the search returned a result

## Commands

`/play [Query]` - Creates a query to search for the inputted song on YouTube to either stream or download it and play it for the user in their voice channel

## Installation

### Prerequisites

- Python3
- A Discord bot token
- The latest version of Ffmpeg

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/jlk31/discord-music-bot.git
   cd discord-music-bot
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root:
   ```
   TOKEN=your_discord_bot_token_here
   ```

4. Run the bot:
   ```bash
   python main.py
   ```

## Getting a Discord Bot Token

1. Go to the [Discord Developer Portal](https://discord.com/developers/applications)
2. Create a new application
3. Navigate to the "Bot" section and create a bot
4. Copy the bot token and add it to your `.env` file
5. Invite the bot to your server using the OAuth2 URL Generator

## Tech Stack

- **Python 3.13**
- **discord.py** - Discord API wrapper
- **python-dotenv** - Environment variable management
- **ffmpeg** - Audio-handling libraries
