# Configuration

Omanges - Streaks Leaderboard is designed so the most common behavior can be changed through Streamer.bot arguments/settings instead of editing C# code.

## Leaderboard settings

The command action includes settings for:

- Number of entries displayed per leaderboard page
- Current-streak leaderboard header text
- Highest-streak leaderboard header text
- Leaderboard entry formatting
- Entry separators
- Empty-leaderboard responses
- Invalid-page responses

## User lookup permissions

`!streak` always allows a viewer to look up their own streak.

The `!streak @username` lookup can be restricted by role using the included permission arguments. Depending on how you configure the extension, access can be granted to roles such as:

- Broadcaster
- Moderator
- VIP
- Subscriber
- Follower
- Everyone

This lets you keep self lookups available while separately controlling who may query other viewers.

## Command responses

Chat messages used by the extension are configurable through arguments so wording can be adjusted without changing the underlying action code.

This includes messages used for:

- Self streak results
- Other-user streak results
- Missing streak data
- Permission failures
- Current-streak leaderboard output
- Highest-streak leaderboard output
- Empty leaderboards
- Invalid leaderboard pages

## Persistent data

Streak data is stored in:

```text
Omanges Extensions/Streaks Leaderboard/streaks.json
```

The JSON file is the persistent source of truth for recorded current and highest streak values.
