# Settings

In Bloxbind 0.2.0 additional settings were added to enable more features and customization.

## Options
Currently two main setting groups exist: Auto Verification and Naming Scheme.

### Auto Verification
- Automatic verification will verify users automatically when they join the server (if enabled).
- When enabled the bot will assign the configured verification role and optionally rename the user (see [Naming Scheme](/settings/#naming-scheme)).

### Naming Scheme
- The naming scheme currently supports a fixed set of options
- Choose one of the following values:
  - "RobloxUsername" - Sets the nickname to the users Roblox username. 
  - "@RobloxUsername" - Sets the nickname to the users Roblox username with an @ symbol prefix. 
  - "RobloxDisplay" - Sets the nickname to the users Roblox display name. 
  - "@RobloxDisplay" - Sets the nickname to the users Roblox display name with an @ symbol prefix. 
  - "DiscordUsername (RobloxUsername)" - Sets the nickname to the users discord username and includes the users roblox username.
  - "DiscordUsername (RobloxDisplay)" - Sets the nickname to the users discord username and includes the users roblox display name.
  - "None" - do not change the user's nickname

#### Examples
Given:
```
Roblox Username: BloxbindRBX
Discord Username: BloxbindDC
Roblox Display Name: BloxbindRBXDisplay
```

- "RobloxUsername" -> BloxbindRBX
- "@RobloxUsername" -> @BloxbindRBX
- "RobloxDisplay" -> BloxbindRBXDisplay
- "@RobloxDisplay" -> @BloxbindRBXDisplay
- "DiscordUsername (RobloxUsername)" -> BloxbindDC (BloxbindRBX)
- "DiscordUsername (RobloxDisplay)" -> BloxbindDC (BloxbindRBXDisplay)
- "none" -> (no nickname change)

#### Notes & limits
- Discord nickname max length: 32 characters. Long generated names may be truncated or rejected.
- To change or view these settings use the `/settings` commands (examples: `/settings key:Auto Verification value:true`, `/settings key:Naming Scheme`).