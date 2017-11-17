here are skinsrestorer commands.
if 

##Table Of Contents
- [User cmds](#User Commands)
- [Admin cmds](#Admin Commands)
- [Config cmds](#Config Commands)


### User Commands
**note that the skinsmenu and skincooldown bypass are not given on op**

if it says you have no permissions to acces these command make sure to read the **bungee install guide**

Command and aliases | Description | Permissions
----------------|--------------|-------
`/skin` | the main command | `skinsrestorer.playercmds` or `OP`
`/skin <skin name>` | changes your skin | `skinsrestorer.playercmds` or `OP`
`/skins` | open the skinsmenu | `skinsrestorer.playercmds.menu`
PERM | bypass the skinscooldown config | `skinsrestorer.bypasscooldown`

### Admin Commands
Command and aliases | Description | Permissions
----------------|--------------|-------
`/sr` | shows the admin command | `skinsrestorer.cmds` or `OP`
`/sr set <player> <skin>` | set's a player skin | `skinsrestorer.cmds` or `OP`
`/sr status` | test the mojang api | `skinsrestorer.cmds` or `OP`
`/sr drop <skin>` | removes the <skin>.SKIN file | `skinsrestorer.cmds` or `OP`
`/sr remove <player>` | removes the <player>.PLAYER file | `skinsrestorer.cmds` or `OP`
`/sr props <player>` | gives the skinprops of the current player | `skinsrestorer.cmds` or `OP`
PERM | bypass the disabledskins list | `skinsrestorer.bypassdisabled` or `OP`

### Config Commands
**note read config guide**

Command and aliases | Description | Permissions
----------------|--------------|-------
`/sr config` `/skinsrestorer config` | show config options | `skinsrestorer.cmds` or `OP`
`/sr reload` | reload and rebuilds the config | `skinsrestorer.cmds` or `OP`
`/sr skinwithoutperm <true/false>` | enable or disable /skin commands without needing perms **bukkit only** | `skinsrestorer.cmds` or `OP`
`/sr SkinExpiresAfter <number>` | set the skinsexpireafter config time **in minutes** read [guide](commands.md) for more info | `skinsrestorer.cmds` or `OP`
`/sr skinCooldown <number>` | set the skin change cooldown time **in seconds** | `skinsrestorer.cmds` or `OP`
`/sr defaultSkins <true/false>` | enabled or disable default skins read (configuring guide defaultskins) |  `skinsrestorer.cmds` or `OP`
`/sr defaultSkins add <skin>` | add a skin to the defaultskin list | `skinsrestorer.cmds` or `OP`
`/sr disabledSkins <true/false>` | block skins from /skin | `skinsrestorer.cmds` or `OP`
`/sr disabledSkins add <skin>` | add a skin to the disabledskin list | `skinsrestorer.cmds` or `OP`
`/sr updater <true/false>` | enable or disable update cheker | `skinsrestorer.cmds` or `OP`


don't use this command unless you want to disable it all
`/sr joinSkins <true/false>` | true => disable skins loading module on join |  `skinsrestorer.cmds` or `OP`
