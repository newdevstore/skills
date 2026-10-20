# New Dev systems catalog

Generated from the dashboard catalog (the same data the MCP `list_systems` tool serves).
IDs are what the MCP tools accept as `systemId`. Free systems run on Lilith; premium ones need an active premium bot.

## Protection

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `antibot` | Anti-BOT | free | Kick Members, View Audit Log | Call set_system_status (writes `defenses.anti.bot`). |
| `antifake` | Anti-Fake | free | Kick Members | Call set_system_status (writes `defenses.anti.fake.status`). |
| `antifiles` | Anti-Files | free | Manage Messages, Kick Members, Timeout Members | Call set_system_status (writes `defenses.anti.files.status`). |
| `antiflood` | Anti-Flood | free | Timeout Members | Call set_system_status (writes `defenses.anti.flood.status`). |
| `antiinvite` | Anti-Invite | free | Manage Messages | Call set_system_status (writes `defenses.anti.invite.status`). |
| `antilink` | Anti-Link | free | Manage Messages | Call set_system_status (writes `defenses.anti.link.status`). |
| `antinuke` | Anti-nuke | free | View Audit Log, Manage Roles | Call set_system_status (writes `status: true` on feature `antinuke`), then fill in the fields with update_system. |
| `antiwebhook` | Anti-webhook | free | Manage Webhooks | Call set_system_status (writes `enabled: true` on feature `antiwebhook`), then fill in the fields with update_system. |
| `automod` | AutoMod | free | Manage Messages, Timeout Members, Kick Members, Ban Members | Call set_system_status (writes `status: true` on feature `automod`), then fill in the fields with update_system. |
| `backup` | Backups | free | Manage Roles, Manage Channels | Call set_system_status (writes `status: true` on feature `backup`), then fill in the fields with update_system. |
| `captcha` | Captcha | free | Manage Roles, Kick Members, Timeout Members, Send Messages, Embed Links | Call set_system_status (writes `status: true` on feature `captcha`), then fill in the fields with update_system. |
| `channelprotection` | Channel Protection | free | View Audit Log, Manage Channels, Manage Roles | Call set_system_status (writes `defenses.anti.channel.status`). |
| `honeypot` | Honeypot | free | Ban Members, Kick Members, Timeout Members, Manage Messages | Call set_system_status (writes `status: true` on feature `honeypot`), then fill in the fields with update_system. |
| `logs` | Logs | free | View Audit Log, View Channels, Send Messages, Embed Links | No single switch: set the channel ID for each log type with update_system (config = { "<logType>": "<channelId>" }). |
| `modprotection` | Moderation Protection | free | View Audit Log, Ban Members, Kick Members, Timeout Members, Manage Roles | Call set_system_status (writes `defenses.anti.moderation.status`). |
| `roleprotection` | Role Protection | free | View Audit Log, Manage Roles | Call set_system_status (writes `defenses.anti.role.status`). |
| `security` | Security Mode | free | Manage Roles, Manage Webhooks | Call set_system_status (writes `status: true` on feature `security`), then fill in the fields with update_system. |
| `antiurl` | URL Protection | premium | View Audit Log, Ban Members, Kick Members, Manage Roles, Send Messages | Call set_system_status (writes `defenses.anti.url.status`). |

## Automations

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `ai` | Artificial Intelligence (under maintenance) | premium | View Channels, Send Messages, Read Message History | Under maintenance: it cannot be enabled right now. |
| `automessage` | Auto Messages | premium | View Channels, Send Messages, Embed Links, Manage Messages | Call set_system_status (writes `enabled: true` on feature `automessage`), then fill in the fields with update_system. |
| `autoreaction` | Auto Reactions | free | View Channels, Add Reactions, Read Message History | Call set_system_status (writes `enabled: true` on feature `autoreaction`), then fill in the fields with update_system. |
| `autorole` | Auto Roles | free | Manage Roles | Call set_system_status (writes `status: true` on feature `autorole`), then fill in the fields with update_system. |
| `sejamembro` | Become a Member | premium | Manage Roles | Call set_system_status (writes `enabled: true` on feature `sejamembro`), then fill in the fields with update_system. |
| `membercounter` | Counters | free | Manage Channels | Call set_system_status (writes `enabled: true` on feature `membercounter`), then fill in the fields with update_system. |
| `giftcards` | Gift Cards | premium | Manage Roles, Send Messages | Call set_system_status (writes `Status: true` on feature `giftcard`), then fill in the fields with update_system. |
| `instagram` | Instagram | premium | View Channels, Send Messages, Manage Messages, Attach Files, Read Message History | No single switch: it is enabled through its configuration (see the guide and currentConfig in get_system). |
| `cl` | My CL | premium | View Channels, Send Messages | Call set_system_status (writes `status: true` on feature `cl`), then fill in the fields with update_system. |
| `barrinhas` | Progress Bars | premium | Manage Roles | Call set_system_status (writes `status: true` on feature `barrinhas`), then fill in the fields with update_system. |
| `verification` | Verification | premium | Manage Roles, Manage Nicknames, Kick Members, Ban Members | Call set_system_status (writes `status: true` on feature `verificacao`), then fill in the fields with update_system. |
| `welcome` | Welcome | free | View Channels, Send Messages, Embed Links, Manage Messages | Call set_system_status (writes `enabled: true` on feature `welcome`), then fill in the fields with update_system. |

## Staff

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `tempcall` | Call Time | free | Manage Channels, Manage Roles, Move Members, Connect, Speak, Video, Use Voice Activity, Priority Speaker | Call set_system_status (writes `Status: true` on feature `tempcall`), then fill in the fields with update_system. |
| `movchat` | Chat Activity | free | View Channels, Read Message History | Call set_system_status (writes `status: true` on feature `movchat`), then fill in the fields with update_system. |
| `meetings` | Meetings | free | View Channels, Send Messages, Embed Links | Call set_system_status (writes `Status: true` on feature `meeting`), then fill in the fields with update_system. |
| `registration` | Registration | free | Manage Roles, Manage Nicknames, View Channels, Send Messages, Embed Links | Call set_system_status (writes `status: true` on feature `registration`), then fill in the fields with update_system. |

## Support

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `recruitment` | Recruitment & Migration | premium | View Channels, Send Messages, Embed Links | No single switch: it is enabled through its configuration (see the guide and currentConfig in get_system). |
| `sellroles` | Role Sales | premium | Manage Roles, Manage Channels, View Channels, Send Messages, Read Message History | Call set_system_status (writes `status: true` on feature `sellroles`), then fill in the fields with update_system. |
| `ticket` | Tickets | premium | Manage Channels, Manage Roles, Create Private Threads, Send Messages in Threads, Manage Threads, View Channels, Send Messages, Embed Links, Attach Files, Read Message History | Call set_system_status (writes `Status: true` on feature `ticket`), then fill in the fields with update_system. |

## VIPs

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `familia` | Family | premium | Manage Roles, Manage Channels, View Channels, Connect, Speak | Call set_system_status (writes `enabled: true` on feature `familia`), then fill in the fields with update_system. |
| `primeiradama` | First Lady | premium | Manage Roles | Call set_system_status (writes `enabled: true` on feature `primeiradama`), then fill in the fields with update_system. |
| `vip` | VIP | premium | Manage Roles, Manage Channels, View Channels, Connect, Speak | Call set_system_status (writes `enabled: true` on feature `vip`), then fill in the fields with update_system. |

## Entertainment

| ID | Name | Tier | Bot permissions | How to enable |
|---|---|---|---|---|
| `counter` | Count Infinitely | free | View Channels, Manage Messages, Add Reactions | Call set_system_status (writes `status: true` on feature `numbercounter`), then fill in the fields with update_system. |
| `economy` | Global Economy | free | View Channels, Send Messages, Manage Roles | Call set_system_status (writes `enabled: true` on feature `economy`), then fill in the fields with update_system. |
| `tellonym` | Tellonym | premium | View Channels, Send Messages, Add Reactions | Call set_system_status (writes `enabled: true` on feature `tellonym`), then fill in the fields with update_system. |
| `xpsystem` | XP | premium | View Channels, Send Messages, Manage Roles | Call set_system_status (writes `enabled: true` on feature `xpsystem`), then fill in the fields with update_system. |
