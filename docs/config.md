# Info

##Table Of Contents
- [Default Config](#Default Config)




## Default Config
the config file can be found on github: [Click Here]: https://github.com/Th3Tr0LLeR/SkinsRestorer---Maro/blob/master/config.yml

here it is also for now:
```json
##############################
#  SkinsRestorer Config.yml  #
##############################
#by Th3Tr0LLeR & Blackfire62 + xknat 

#This option disables automatic requesting & applying skins on join.
#Commands still work!
DisableOnJoinSkins: false

#enables /skin without permissions
#(only works for backend aka spigot servers)
SkinWithoutPerm: false

#How long the skin will be in the database (in minutes)
SkinExpiresAfter: 5

#This is for preventing skin change spam (in seconds)
#[skinsrestorer.bypasscooldown bypasses this]
SkinChangeCooldown: 30
 
#Enable or disable default skins
#If more nicknames will be in the list, server will always choose a random one.
DefaultSkins:
  Enabled: false
  Names:
    - Steve
    
#Disable skin names
#Put skins you want to disable on the list
#Player wont be able to set these skins
#[skinsrestorer.bypassdisabled bypasses this]
DisabledSkins:
  Enabled: false
  Names:
    - Steve
    
#Multi-Bungee support
#If you use more proxy servers and you
#experience issues with skin visibility between proxies?
#enable this option!
#(RedisBungee enables this option automatically)
MultiBungee:
  Enabled: false

# MySQL database for large servers
# or just to boost the performance
MySQL:
  Enabled: false
  Host: localhost
  Port: 3306
  Database: db
  SkinTable: Skins
  PlayerTable: Players
  Username: root
  Password: pass

#Enable or disable the updater check.
Updater:
  Enabled: true
```
###end
