# 3DS-Presence
[Website](https://3ds-presence.top/) | [Discord](https://discord.gg/npkgkVgzWF)

Display the game you are playing on your Nintendo 3DS in your Discord status.

## How it works

A custom firmware based on Luma3DS detects the current game on the console and sends its title, publisher and ID to a server. The server generates a Discord Rich Presence activity and posts it to your profile through the Discord API.

Some games can also provide extra information about the current state of the game (like level, score, etc.) for a more detailed activity.

## Getting started

- **Official website**
    - Visit [3ds-presence.top](https://3ds-presence.top/) to get your configuration file and follow the installation guide
- **Self-hosting**
    - See the [Presence-Server](https://github.com/3ds-presence/Presence-Server) README to deploy your own infrastructure


## Repositories

| Repo | Role |
|---|---|
| [Presence3DS](https://github.com/3ds-presence/Presence3DS) | Custom firmware (Luma3DS fork) that detects and sends the current game |
| [Presence-Server](https://github.com/3ds-presence/Presence-Server) | Docker orchestration for the full infrastructure |
| [Presence-Backend](https://github.com/3ds-presence/Presence-Backend) | API: Discord authentication, token management, Gateway connection |
| [Activity-Generator](https://github.com/3ds-presence/Activity-Generator) | Rich Presence activity generation (basic and advanced Lua scripts) |
| [Presence-Frontend](https://github.com/3ds-presence/Presence-Frontend) | Website: Discord login, configuration download, game logos |

## Contributing

- **Add game logos** in the [Presence-Frontend](https://github.com/3ds-presence/Presence-Frontend)
- **Write Lua scripts** to enhance a game's activity, see [Activity-Generator](https://github.com/3ds-presence/Activity-Generator) and [RPC-AddOns](https://github.com/3ds-presence/RPC-AddOns)
- **Report a bug** by opening an issue in the relevant repository