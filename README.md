# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) preset for herbertkokholm repos.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["local>herbertkokholm/renovate-config"]
}
```

- Runs in the first week of each month (Europe/Copenhagen); security fixes come immediately.
- Non-major updates grouped into one PR; GitHub Actions in their own PR, pinned to commit SHA.
- Major updates wait for approval in the Dependency Dashboard.
- New releases must be 3 days old before they are proposed.
