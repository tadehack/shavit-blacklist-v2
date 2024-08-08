# Shavit Blacklist v2  
This is an improved version of the blacklist plugin for shavit's timer, most of the changes where made by [enimmy](https://github.com/enimmy), I only added some bonus features on top and changed a few things :)

## Features (and changes):  

### Enimmy changes:  
- Integrated SouceJump bans API > Automatically inserts a banned user in the blacklist (manual insertion is also available with the command: sm_blm *steamid*, or by manually searching through the list ('blm' stands for 'blacklist menu')).  
  
- Support for multiple blacklisted styles instead of just one.

  
  ### My changes:  
- Alongside the 'blacklist' special string, there is now a new 'blacklistOnly' special string, when inserting this new special string on a style, it will make it so only who are blacklisted can play on that style, while with the old 'blacklist' special string, both blacklisted and non-blacklisted players can play on that style. This is useful when you still want to let blacklisted players play on some of the off-styles while at the same time having their unique blacklisted-only styles, example: 'Blacklist Normal' and 'Blacklist Segmented' will use the 'blacklistOnly' special string, while styles like 'TAS' and 'Parkour' can have the regular 'blacklist' special string.  
  
- If a blacklisted player switch their style to a non-blacklisted style and a 'blacklistOnly' style exists, their style will be changed to the first 'blacklistOnly' style on the list, if not, their style will be changed to the first regular 'blacklist' style on the list.  
  
- The /blacklist command was changed to /blacklistmenu, /blmenu or /blm, the reason for that is so you can have the /blacklist command for the default blacklist style, that way it won't overlap with the admin command.

- Some of the plugin texts were re-writen for a cleaner look.
