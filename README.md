Psycho-Core-7.3.5 — Legion
A modernized TrinityCore-based emulator for World of Warcraft: Legion (7.3.5).

What this is
A World of Warcraft: Legion 7.3.5 private-server emulator descended from TrinityCore.

This is not a binary release — you compile it yourself from this repository against your own dependencies and feed it the data files (maps, vmaps, mmaps, DB2/DBC) extracted from a real Legion 7.3.5 WoW client.

Configuration
Two config files:

worldserver.conf.dist — Game rules, network, rates, and tuning settings. Copy to worldserver.conf and edit.

bnetserver.conf.dist — Battle.net auth server config. Copy to bnetserver.conf and edit.

Key knobs you'll touch first:

Ini, TOML
# Database connection strings
LoginDatabaseInfo     = "127.0.0.1;3306;psycho;core;psycho_auth"
CharacterDatabaseInfo = "127.0.0.1;3306;psycho;core;psycho_characters"
HotfixDatabaseInfo    = "127.0.0.1;3306;psycho;core;psycho_hotfixes"
WorldDatabaseInfo     = "127.0.0.1;3306;psycho;core;psycho_world"

# Where extracted client data lives
DataDir = "."

# Expansion (Legion = 6)
Expansion = 6
License
This repository is licensed under GPL-2.0-or-later (see COPYING).
