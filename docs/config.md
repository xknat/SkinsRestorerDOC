# Info

###Table Of Contents
- [Config guide](#config-guide)

    [reducing api request](#reducing-api-request)
    
    [apply custom default skins](#apply-custom-default-skins)
    
    
- [Default Config](#default-config)


## Config Guide

We want skinsrestorer to be ease of use. thats why it there are little advanced config option.

the plugin should be able to run without config needed but if you feel like you need it then your at the right place here.

here are some little tips:

### Reducing api request

a lot of big server owners want to reduce api usage to increase performance. you can do this by the following:

1. set the "skinsexpireafter" higher

2. set the "skincooldown" higher 

3. only make skinchange available for donators 


### Apply custom default skins
**not working for bungee on version 13.1.4-BETA or below**

if you want to apply a default skin for your server you can do the following:

1. set the skin on your own using /skin to load it in the database

1.2 [optional] you can sure the skin does not change by setting the 3th row of the skin to 2524608000 (wich is year 2050) [this will also reduce api skinrequest]

2. set the defaultskins on true and add the disired skin

3. restart the or do "/sr reload"


done!

-----------------

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
