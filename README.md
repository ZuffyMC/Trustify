<div align="center">

![Trustify Banner](https://cdn.modrinth.com/data/cached_images/a169470db4bf2398aeb7451006493786b06d1155_0.webp)

# Trustify Version 1.0

### Smart Reputation, Trust & Karma System for Minecraft Servers

![Minecraft](https://img.shields.io/badge/Minecraft-1.21%2B-brightgreen?style=for-the-badge)
![Java](https://img.shields.io/badge/Java-21%2B-orange?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Paper-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Beta-yellow?style=for-the-badge)

**Trustify** is a modern Minecraft plugin designed to help servers build a safer, healthier, and more positive community through reputation, trust, karma, ratings, leaderboards, rewards, and community safety tools.

Track player reputation, trust level, karma, ratings, helpful actions, chat behavior, and suspicious activity in one lightweight and fully configurable system.

</div>

---

## ✨ Overview

Trustify helps server owners identify which players are trusted, friendly, helpful, suspicious, or dangerous.

Players can gain reputation by helping newcomers, behaving positively, receiving good ratings, answering questions, and contributing to the community.

Negative behavior such as toxic chat, suspicious activity, repeated targeting, scam reports, and harmful actions can reduce trust and karma.

Trustify is built for survival, SMP, economy, roleplay, and community-based servers that want to reward helpful players while protecting newcomers from risky interactions.

---

## 🌟 Core Features

### ⭐ Reputation System
Players gain reputation based on positive community actions such as helping new players, receiving good ratings, answering questions, and being active in a positive way.

### 🛡 Trust System
Each player has a trust level that shows how safe or risky they are. Trust can increase through helpful behavior and decrease from negative actions.

### ⚖ Karma System
Karma represents the overall behavior of a player. Good actions increase karma, while harmful actions reduce it.

### 🤝 Helpful Player Detection
Trustify can detect helpful actions such as assisting new players, giving useful items, answering questions, and supporting the server community.

### 💬 Chat Behavior Scanner
The plugin can scan chat behavior using configurable keyword rules to detect positive, toxic, spam, or suspicious messages.

### ⚔ Combat Trust Detection
Killing new players or repeatedly targeting the same player can reduce trust, while PvP arenas, duel zones, or ignored worlds can be excluded.

### ⭐ Player Rating System
Players can rate others through commands or GUI. Ratings can affect reputation, trust, and karma.

### 🏆 Leaderboards
Show top players based on reputation, trust, karma, ratings, and helpful actions.

### 🎁 Reward System
Reward trusted, helpful, and positive players with configurable commands, permissions, ranks, money, items, or cosmetics.

### 🧩 PlaceholderAPI Support
Display Trustify data on scoreboards, tablists, chat formats, holograms, menus, and more.

### ⚙ Fully Configurable
Almost everything can be customized, including scores, status levels, GUI layouts, messages, rewards, modules, cooldowns, and performance settings.

---

## 🖥 GUI System

Trustify includes a full GUI system designed to be clean, modern, and easy to use.

Included GUI menus:

- Dashboard
- Player Profile
- Player Rating
- Online Player Rating List
- Leaderboards
- Trust Guide
- Rewards
- Help Center
- Admin Dashboard
- Player Inspect
- Logs
- Performance
- Module Status

All GUI text supports language switching and can be configured through message files.

---

## 🛡 Trust Status Examples

| Status | Meaning |
| --- | --- |
| 🟢 **Trusted** | Safe, helpful, and positive player |
| 🔵 **Friendly** | Generally good and friendly |
| ⚪ **Neutral** | Not enough data yet |
| 🟡 **Suspicious** | Some negative behavior detected |
| 🔴 **Dangerous** | Be careful when interacting with this player |

---

## 📦 Commands

### Player Commands

```text
/trustify
/trustify profile
/trustify <player>
/trustify rating
/trustify rating <player>
/trust <player>
/karma <player>
/rate <player>
/top trustify
/top trusted
/top karma
```

### Admin Commands

```text
/trustifyadmin
/trustifyadmin gui
/trustifyadmin reload
/trustifyadmin set <player> reputation <amount>
/trustifyadmin set <player> trust <amount>
/trustifyadmin set <player> karma <amount>
/trustifyadmin add <player> <type> <amount>
/trustifyadmin reset <player>
/trustifyadmin logs <player>
/trustifyadmin debug <player>
/trustifyadmin performance
/trustifyadmin cache
/trustifyadmin queue
/trustifyadmin timings
```

---

## 🔐 Permissions

```text
trustify.use
trustify.profile.others
trustify.rate
trustify.top
trustify.admin
trustify.admin.reload
trustify.admin.set
trustify.admin.reset
trustify.admin.logs
trustify.admin.performance
trustify.bypass.cooldown
trustify.combat.bypass
trustify.newbie.bypass
trustify.leaderboard.hide
```

---

## 🧩 PlaceholderAPI Placeholders

```text
%trustify_score%
%trustify_status%
%trustify_trust_score%
%trustify_trust_status%
%trustify_karma_score%
%trustify_karma_status%
%trustify_rating_average%
%trustify_rating_count%
%trustify_helped_newbies%
%trustify_rank_trustify%
%trustify_rank_trust%
%trustify_rank_karma%
```

---

## ⚙ Performance First

Trustify is designed to be lightweight and optimized.

The plugin uses:

- Async database operations
- Cached player profiles
- Leaderboard cache
- Batch saving
- Cooldowns and daily limits
- Configurable performance modes
- Optional modules that can be enabled or disabled

Performance modes:

```text
LIGHT
BALANCED
DETAILED
```

---

## 🔌 Supported Integrations

Trustify can work with:

- PlaceholderAPI
- Vault
- LuckPerms
- WorldGuard
- EssentialsX
- CombatLogX
- Lands
- GriefPrevention
- DiscordSRV

All integrations are optional and can be configured.

---

## 💾 Storage

Supported storage types:

```text
SQLite
MySQL
```

Runtime data is stored cleanly inside:

```text
plugins/Trustify/data/
```

Example structure:

```text
plugins/Trustify/
├── config.yml
├── layout.yml
├── status.yml
├── rewards.yml
├── permissions.yml
├── integrations.yml
├── data/
│   ├── database.db
│   └── backups/
├── messages/
│   ├── english.yml
│   └── indonesia.yml
└── modules/
    ├── chat.yml
    ├── rating.yml
    ├── trust.yml
    ├── newbie.yml
    └── combat.yml
```

---

## 🌐 Language Support

Default message files:

```text
messages/english.yml
messages/indonesia.yml
```

Changing the language in `config.yml` also changes GUI text, item names, lore, command feedback, admin messages, and status descriptions.

```yaml
settings:
  language: "english"
```

Available values:

```text
english
indonesia
```

---

## 🎁 Reward System

Server owners can reward players based on:

- High reputation
- Trusted status
- Weekly leaderboard position
- Karma milestones
- Helpful behavior
- Rating achievements

Rewards can run commands such as giving money, permissions, ranks, items, or cosmetics.

---

## ✅ Perfect For

Trustify is great for:

- Survival servers
- SMP servers
- Economy servers
- Roleplay servers
- Community servers
- Newbie-friendly servers
- Servers that want a safer social system

---

## 📌 Requirements

```text
Minecraft: 1.21+
Java: 21+
Server Software: Paper recommended
```

Spigot compatibility may depend on enabled features and server environment.

---

## 📥 Download

Trustify is distributed through Modrinth.

> This repository is used for plugin information, documentation, updates, and issue tracking.  
> The source code is not publicly available.

---

<div align="center">

**Trustify**  
Build a safer and more trusted Minecraft community.

</div>
