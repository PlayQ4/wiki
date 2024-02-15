# Q4Max commands

## Index
- [Commands](#commands)
  - [Client](#client-commands)
  - [Referee](#referee-commands)
  - [Server](#server-commands)
 
## Commands

### Client commands
| Command | Parameters | Summary | Description | Type |
| --- | --- | --- | --- | --- |
| _button1 |  | Allows a coach to send voice chat to the currently spectated player. | This functions like press-to-talk voice chat, with the only exception that it only sends messages to the player you are currently viewing. | ![client](https://img.shields.io/badge/Client-blue) |
| autorecord |   | Records a netdemo with a name in the same format as autoaction recorded demos. | This behaves like "recordnetdemo", except it does not take any arguments : it will name the recorded demo in the same format as autoaction demos. | ![client](https://img.shields.io/badge/Client-blue) |
| aviNetDemo | \<a netdemo filename\> | Capture screenshots from a netdemo suitable for creating an avi. | This command will turn an entire netdemo into a sequence of tga or jpg screenshots running at 62.5 fps. When executed, this will set demo_aviDemoName to the filename passed as a parameter and save the screenshots in a subdirectory of q4max/screenshots/avidemo/ named after this filename. It will keep going as long as demo_aviDemoScreenshots is set to 1, or until you disconnect/the demo ends. | ![client](https://img.shields.io/badge/Client-blue) |
| callvote | \<votename\> [setting] | Calls a vote on a given option. | This allows a player to vote for a specific setting to be changed. The <votename> parameter indicates what is voteable, and the [setting] parameter indicates the value requested. There are many voteable settings - these can be listed, complete with a description using "callvote ?". See [the current list of settings](votes_en.md). Using this command with no [setting] parameter will display the current state of this setting. Note that server operators can disable specific votes if they do not wish any given setting to be voteable. Common votes include "callvote mode CA" or "callvote map mp/swq4dm1". | ![client](https://img.shields.io/badge/Client-blue) |
| cancelcoach |  | Makes you quit your coaching position. | Use this if you want to quit coaching a team. | ![client](https://img.shields.io/badge/Client-blue) |
| coach |   | Accepts a coaching invitation. | Issuing this command turns you into a coach for the team which sent the invitation. As a coach, you can partake in the team's teamchat (both in type and using voicechat), see the team overlay and view any players on the coached team. You can also use the _button1 to send voice messages to the player you are currently viewing. | ![client](https://img.shields.io/badge/Client-blue) |
| coachdecline |   | Declines a coaching invitation. |   | ![client](https://img.shields.io/badge/Client-blue) |
| coachinvite | \<playerid\> | Invites a player to coach your team. | Invites a spectator to coach your team. Get the spectator's player id by using the players command. | ![client](https://img.shields.io/badge/Client-blue) |
| coachrevoke |   | Revokes a coach. | Use this if you want to remove a coach from your team. | ![client](https://img.shields.io/badge/Client-blue) |
| demoSlowDown |   | Slow down netdemo playback. | This command halves demo_scale down to 0.25. | ![client](https://img.shields.io/badge/Client-blue) |
| demoSpeedReset |   | Reset netdemo playback to normal speed. | This command resets demo_scale to 1. | ![client](https://img.shields.io/badge/Client-blue) |
| demoSpeedUp |   | Speedup netdemo playback. | This command doubles demo_scale up to 32. | ![client](https://img.shields.io/badge/Client-blue) |
| fixUserInfo |   | Attempts to get your userInfo from the server. | If using the command once doesn't help, don't bother spamming it - it will either work, or it wont. | ![client](https://img.shields.io/badge/Client-blue) |
| follow | \<powerup\> or \<playerid\> | Allows a spectator to switch to a nominated player when spectating. | This allows a spectator to follow either a specific player, or to follow a player holding a specific powerup. The parameter can either be one of the powerup names ("quad", "regen", "haste", "invis", "marineflag" or "stroggflag"), or the player id reported by the "players" command for the player you wish to follow. If there are multiple powerups of the same type in play at the same time, executing this command multiple times will cycle through all players with that powerup. Note that this is not "automatic" following of the powerups, and simply changes to the player holding that powerup at the time you execute this command. | ![client](https://img.shields.io/badge/Client-blue) |
| lockteam |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| maplist |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| multipov |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| networkStats |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| players |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| referee |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| reloadHud |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| specinvite |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| speclock |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| specrevoke |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| teamready |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| timein |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| timeout |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| viewSizeUp/viewSizeDown |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| weapon |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |

### Referee commands

| Command | Parameters | Summary | Description | Type |
| --- | --- | --- | --- | --- |
| abort |  | Abandons the current game and returns to warmup. | This command is intended to be used when a match needs to be abandoned. It sets all players to "not ready", and resets the game back to the warmup. | ![referee](https://img.shields.io/badge/Referee-orange) |
| allready |   | Readies up all players and begins the game. | This forces all players to be "ready", even if they have not readied up themselves, thus allowing the game to begin. | ![referee](https://img.shields.io/badge/Referee-orange) |
| cancelref |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| coachMarine |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| coachStrogg |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| ingame |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| lockteams |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| marine |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| pause |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| remove |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specBoth |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specMarine |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specStrogg |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| speclockall |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| speclockmarine |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| speclockstrogg |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specunlockall |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specunlockmarine |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| specunlockstrogg |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| strogg |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| unlockteams |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |
| unpause |   |   |   | ![referee](https://img.shields.io/badge/Referee-orange) |

### Server commands


| Command | Parameters | Summary | Description | Type |
| --- | --- | --- | --- | --- |
| addBot | \<name\> \<team\> | Add a bot. | Add a "name" bot. If the name matches a defined bot personality, the defined bot will be added, otherwise it will be a default bot. In team games, you can also specify the team (strogg or marine, marine if unspecified). | ![server](https://img.shields.io/badge/Server-green) |
| AddGuidToBanList | \<GUID\> | Adds a GUID into the banlist. | Adds the given GUID into the banlist. The guid is a q4 guid, as shown by the players command. Another useful source of of player to GUID mappings is from the stats XML logs. If the guid contains non-alpha chars, it is worth quoting the parameter to make sure it is entered correctly. | ![server](https://img.shields.io/badge/Server-green) |
| AddIPToBanList | \<IP\> | Adds an IP into the banlist. | Adds the IP into the banlist. If the ip is just the beginning of the IP (eg 123.123.123) then it will ban 123.123.123.* - do not use wildcards though, its automatic. Note that you must use the IP as displayed in the q4 console at connection - this is usually dotted quads, but it is sometimes resolved in the case of localhost, and maybe other computers on the sam LAN. | ![server](https://img.shields.io/badge/Server-green) |
| broadcastMsg |   | Broadcast a message to all clients. | Sends a string to clients, which will show in the MOTD field. Useful for "shutting down server!" warnings or TV centerprints. | ![server](https://img.shields.io/badge/Server-green) |
| networkStats |   | Report network traffic stats. | On a client, reports in/out rate and incoming PL to the console. On a server, reports in/out rate and incoming PL of each client to the server console. | ![server](https://img.shields.io/badge/Server-green) |
| passvote |   | Pass a vote. | This is used to pass votes straight from the server console. | ![server](https://img.shields.io/badge/Server-green) |
| RemoveGuidFromBanList | \<GUID\> | Removes a GUID from the banlist. | Removes the given GUID from the banlist. Only exact matches are removed, so be careful to type it exactly as entered in the ban list. As with adding, make sure that the guid is quoted if contains slashes etc. | ![server](https://img.shields.io/badge/Server-green) |
| RemoveIPFromBanList | \<IP\> | Removes an IP from the banlist. | Removes an IP from the banlist. Only exact matches are removed, so be careful to type it exactly as entered in the ban list. This includes partial IPs used to ban entire ranges of IPs. | ![server](https://img.shields.io/badge/Server-green) |
| ShowBanList | \<GUID\> | Displays the banlist. | This command can be used to look at the players that are currently entered into the banlist, listing name (if known), guid. IP bans are shown with a blank guid, and a name of the IP that is banned. | ![server](https://img.shields.io/badge/Server-green) |
