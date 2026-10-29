<div align="center">
  <img src="https://raw.githubusercontent.com/Reyyzxx01/ChatHook/main/logo.png" width="160" alt="ChatHook Logo">

  <h1>ChatHook</h1>

  <p>ChatHook is a lightweight Paper plugin that relays in-game chat straight to your Discord server via webhook, with a clean <code>[player] [time] message</code> format.</p>

  <a href="https://github.com/Reyyzxx01/ChatHook/raw/refs/heads/main/ChatHook-1.0.jar">
    <img src="https://img.shields.io/badge/Download-ChatHook-8b5cf6?style=for-the-badge&logo=github" alt="Download ChatHook">
  </a>
</div>

## Preview
Player `gom` types `hi` in game -> Discord shows:

```
[gom] [22:38] hi
```

## Features
- Plain in-game chat to Discord, format fully configurable (`[%player%] [%time%] %message%`)
- Configurable timezone and time format (empty timezone = server timezone)
- `@everyone` / `@here` / role pings from chat never ping anyone
- Async webhook requests (no server lag) with rate-limit retry
- Works with Floodgate (Bedrock) names as they appear in game

## Commands (OP / console only, permission `chathook.admin`)
| Command | Description |
|---|---|
| `/chathook enable` | Enable sending (saved in config) |
| `/chathook disable` | Disable sending (saved in config) |
| `/chathook reload` | Reload `config.yml` |
| `/chathook version` | Show version and links |

## Setup
1. Drop the jar into `plugins/` and start the server once.
2. Set `webhook-url` in `plugins/ChatHook/config.yml`.
3. Run `/chathook reload`.

## Build
Requires Java 21 and Maven: `mvn package`

## Links
- GitHub: https://github.com/Reyyzxx01/ChatHook
- Web: https://reyyzxx01.vercel.app

## Credits
Created by [Reyyzxx01](https://github.com/Reyyzxx01). If you fork or redistribute this plugin, please keep this credit.
