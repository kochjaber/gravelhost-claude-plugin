# GravelHost

Check, fix and manage your GravelHost game servers from a conversation with Claude.

## What it does

The plugin connects Claude to your GravelHost account through the GravelHost connector (`https://mcp.gravelhost.com/mcp`) and adds six skills that teach Claude how to work on game servers and websites:

- **server-doctor**: finds why a server is down, crashing, lagging or refusing players, from its console and resource use, and proposes a fix.
- **safe-changes**: backup first, warn players before restarts, ask before anything that can't be undone, and confirm the result.
- **minecraft-content**: installs, updates and removes plugins and mods that fit the server's loader and version.
- **player-moderation**: whitelist, operators, bans, kicks and announcements.
- **support-ticket**: opens a support ticket with the case already written, follows the replies.
- **website-care**: site and certificate problems, PHP, email, DNS and backups of web hosting.

Commands: `/gravelhost:diagnose` and `/gravelhost:status`.

## Install

- **Claude Code:** `/plugin marketplace add kochjaber/gravelhost-claude-plugin`, then `/plugin install gravelhost@gravelhost`.
- **Connector only** (claude.ai, Claude Desktop, any MCP app): add a custom connector with the address `https://mcp.gravelhost.com/mcp`.

## Use it

1. Install the plugin, then connect the GravelHost connector from the plugin's Connectors tab.
2. Sign in to the GravelHost panel when asked, and choose what Claude may do (view, power and console, files and content, backups, settings, support tickets, websites) and on which servers.
3. Ask things like "Why does my Minecraft server keep crashing?", "Make a backup and install LuckPerms", or "Set max players to 40".

You can see and disconnect your AI apps at any time on the panel: https://panel.gravelhost.com/ai-connections

## Data

Claude reads and changes only the servers and permissions you approve, with your own panel permissions. What the tools return (status, console lines, file contents, settings) goes to Claude to answer you. Passwords, keys and tokens in startup settings and in files (shown as "(hidden)"), database passwords, account details and billing are never sent. Anything that can't be undone needs your yes first. GravelHost logs each action (tool, server, time, result) for 90 days so you can see what your AI apps did. The plugin itself stores nothing.

Support: https://gravelhost.com/contact · Privacy: https://gravelhost.com/legal#privacy
