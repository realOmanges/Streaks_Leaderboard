# Omanges - Streaks Leaderboard

A Streamer.bot extension for tracking Twitch watch streaks, looking up viewer streaks, and displaying current or all-time streak leaderboards in chat.

## Features

- Tracks Twitch watch streak events automatically
- Stores each viewer's current streak and highest recorded streak
- `!streak` lookup for the current user
- Optional `!streak @user` lookup with configurable permissions
- Current-streak leaderboard
- Highest-streak leaderboard
- Pagination support
- Configurable leaderboard page size
- Customizable chat formatting and response text
- Persistent JSON storage

## Commands

| Command | Description |
| --- | --- |
| `!streak` | Shows your current and highest streak |
| `!streak @username` | Looks up another viewer's streak if permitted |
| `!streak leaderboard [page]` | Displays the current-streak leaderboard |
| `!streak highest [page]` | Displays the highest-streak leaderboard |

## Data Storage

The extension stores its data in:

```text
Streamer.bot/
└── Omanges Extensions/
    └── Streaks Leaderboard/
        └── streaks.json
```

The data file is created and maintained automatically by the extension.

## Installation

1. Download the latest `.sb` export from the GitHub Releases page.
2. Open Streamer.bot.
3. Import the `.sb` file.
4. Review the extension arguments/settings and adjust permissions or formatting as desired.
5. Confirm the included Twitch watch-streak trigger is enabled.

See [`docs/SETUP.md`](docs/SETUP.md) for more details.

## Configuration

The extension exposes configurable arguments for permissions, leaderboard size, and chat formatting.

See [`docs/CONFIGURATION.md`](docs/CONFIGURATION.md) for a settings overview.

## Version

Current documented release: **v1.0.1**

See [`CHANGELOG.md`](CHANGELOG.md) for release history.

## Requirements

- Streamer.bot 1.0.4 or newer recommended
- Twitch account connected to Streamer.bot
- Twitch watch-streak events available to the broadcaster/account

## License

This project is licensed under the MIT License. See [`LICENSE`](LICENSE).
