# TRF ON TOP — Discord Multi-Bot Controller & Music System

TRF-branded build of the supplied Discord bot project.

## Deploy on Railway (phone-friendly)

1. Upload this project to a GitHub repository.
2. Create a Railway project from that repository.
3. In Railway → Variables, add `DISCORD_TOKEN` with your **newly reset** Discord bot token.
4. Add `OWNER_ID` with your Discord user ID.
5. Deploy. Railway uses the included `Dockerfile` and `railway.toml`.

**Never put your bot token in `config.json`, source code, GitHub, or chat.**
The `.env.example` file is only a template; do not put a real token in it.

## Features retained

- Multi-bot connection support (`BOT_TOKENS`, optional)
- Music playback and queue controls
- Voice join / leave / follow / jump controls
- Bot profile, avatar, banner, username and bio commands
- Owner and trusted-admin controls
- Status, bot info and help commands
- Prefix commands (default `.`)

Mass-message `.spam` and `.dmspam` commands are disabled in this TRF build.

## Requirements

Node.js 20+ and FFmpeg (provided by the Docker image).
