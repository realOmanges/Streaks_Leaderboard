# Setup

## 1. Import the extension

1. Download the latest `.sb` file from GitHub Releases.
2. Open Streamer.bot.
3. Use **Import** and select the downloaded `.sb` file.
4. Confirm the imported actions and triggers are enabled.

## 2. Verify the included actions

The extension contains two primary actions:

- `!streak`
- `Twitch Watch Streak - Record`

The record action handles Twitch watch-streak events and writes viewer streak data to JSON. The command action handles viewer lookups and leaderboards.

## 3. Data location

The extension stores persistent data at:

```text
Streamer.bot/
└── Omanges Extensions/
    └── Streaks Leaderboard/
        └── streaks.json
```

Do not manually edit the file while Streamer.bot is actively writing to it unless you have stopped the relevant actions first.

## 4. Test the extension

After Streamer.bot has recorded at least one watch-streak event, test:

```text
!streak
!streak leaderboard
!streak highest
```

If `@user` lookups are enabled for your role, also test:

```text
!streak @username
```

## 5. Adjust settings

Review the arguments/settings attached to the command action. These control lookup permissions, leaderboard page size, and response formatting.

See [`CONFIGURATION.md`](CONFIGURATION.md) for details.
