# Q4Max commands

## Index
- [Commands](#commands)
- [Details](#details)
  - [Client](#client-commands)
  - [Referee](#referee-commands)
  - [Server](#server-commands)
 
## Commands
| Command | Summary | Type |
| --- | --- | --- |
| [_button1](#_button1) | Allows a coach to send voice chat to the currently spectated player. | ![client](https://img.shields.io/badge/Client-blue) |
| [autorecord](#autorecord) | Records a netdemo with a name in the same format as autoaction recorded demos. | ![client](https://img.shields.io/badge/Client-blue) |
| [aviNetDemo](#avinetdemo) | Capture screenshots from a netdemo suitable for creating an avi. | ![client](https://img.shields.io/badge/Client-blue) |
| [callvote](#callvote) | Provides a way to vote for many votable options. | ![client](https://img.shields.io/badge/Client-blue) |
| [cancelcoach](#cancelcoach) | Makes you quit your coaching position. | ![client](https://img.shields.io/badge/Client-blue) |
| [coach](#coach) | Accepts a coaching invitation. | ![client](https://img.shields.io/badge/Client-blue) |
| [coachdecline](#coachdecline) | Declines a coaching invitation. | ![client](https://img.shields.io/badge/Client-blue) |
| [coachinvite](#coachinvite) | Invites a player to coach your team. | ![client](https://img.shields.io/badge/Client-blue) |
| [coachrevoke](#coachrevoke) | Revokes a coach. | ![client](https://img.shields.io/badge/Client-blue) |
| [demoSlowDown](#demoslowdown) | Slow down netdemo playback. | ![client](https://img.shields.io/badge/Client-blue) |
| [demoSpeedReset](#demospeedreset) | Reset netdemo playback to normal speed. | ![client](https://img.shields.io/badge/Client-blue) |
| [demoSpeedUp](#demospeedup) | Speedup netdemo playback. | ![client](https://img.shields.io/badge/Client-blue) |
| [fixUserInfo](#fixuserinfo) | Attempts to get your userInfo from the server. | ![client](https://img.shields.io/badge/Client-blue) |
| [follow](#follow) | Allows a spectator to switch to a nominated player when spectating. | ![client](https://img.shields.io/badge/Client-blue) |
| [lockteam](#lockteam) | Locks/unlocks your team from players. | ![client](https://img.shields.io/badge/Client-blue) |
| [maplist](#maplist) | Lists all the maps available on the server. | ![client](https://img.shields.io/badge/Client-blue) |
| [multipov](#multipov) | Allows a spectator to view all members of a team at once. | ![client](https://img.shields.io/badge/Client-blue) |
| [networkStats](#networkstats) | Report network traffic stats. | ![client](https://img.shields.io/badge/Client-blue) |
| [players](#players) | Lists all players, and a unique player id to use with other commands. | ![client](https://img.shields.io/badge/Client-blue) |
| [referee](#referee) | Used to make yourself a referee, granting limited admin rights. | ![client](https://img.shields.io/badge/Client-blue) |
| [reloadHud](#reloadhud) | Reloads the current hud. | ![client](https://img.shields.io/badge/Client-blue) |
| [specinvite](#specinvite) | Invites a player to spectate your team. | ![client](https://img.shields.io/badge/Client-blue) |
| [speclock](#speclock) | Locks/unlocks your team from spectators. | ![client](https://img.shields.io/badge/Client-blue) |
| [specrevoke](#specrevoke) | Revokes an invited spectator of your team. | ![client](https://img.shields.io/badge/Client-blue) |
| [teamready](#teamready) | Marks everyone on your team as ready. | ![client](https://img.shields.io/badge/Client-blue) |
| [timein](#timein) | Calls the end of a timeout. | ![client](https://img.shields.io/badge/Client-blue) |
| [timeout](#timeout) | Calls a timeout | ![client](https://img.shields.io/badge/Client-blue) |
| [viewSizeUp/viewSizeDown](#viewsizeup/viewsizedown) | Increase/decrease view size. | ![client](https://img.shields.io/badge/Client-blue) |
| [weapon](#weapon) | Switches to the given weapon | ![client](https://img.shields.io/badge/Client-blue) |
| [abort](#abort) | Abandons the current game and returns to warmup. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [allready](#allready) | Readies up all players and begins the game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [cancelref](#cancelref) | Makes you quit your referee position. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [coachMarine](#coachmarine) | Assign a given player to coach duty for the marine team. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [coachStrogg](#coachstrogg) | Assign a given player to coach duty for the strogg team. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [ingame](#ingame) | Puts a given player in a non-team game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [lockteams](#lockteams) | Locks teams to prevent players joining mid-game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [marine](#marine) | Puts a given player on the marine team. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [pause](#pause) | Pauses a game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [remove](#remove) | Removes a given player from a game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specBoth](#specboth) | Turn a given player into an all-seeing spectator. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [speclockall](#speclockall) | Locks both teams from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [speclockmarine](#speclockmarine) | Locks the Marine team from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [speclockstrogg](#speclockstrogg) | Locks the Strogg team from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specMarine](#specmarine) | Turn a given player into a marine spectator. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specStrogg](#specstrogg) | Turn a given player into a strogg spectator. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specunlockall](#specunlockall) | Unlocks both teams from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specunlockmarine](#specunlockmarine) | Unlocks the Marine team from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [specunlockstrogg](#specunlockstrogg) | Unlocks the Strogg team from spectators. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [strogg](#strogg) | Puts a given player on the strogg team. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [unlockteams](#unlockteams) | Unlocks teams to allow players to join. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [unpause](#unpause) | Unpauses a game. | ![referee](https://img.shields.io/badge/Referee-orange) |
| [addBot](#addbot) | Add a bot. | ![server](https://img.shields.io/badge/Server-green) |
| [AddGuidToBanList](#addguidtobanlist) | Adds a GUID into the banlist. | ![server](https://img.shields.io/badge/Server-green) |
| [AddIPToBanList](#addiptobanlist) | Adds an IP into the banlist. | ![server](https://img.shields.io/badge/Server-green) |
| [broadcastMsg](#broadcastmsg) | Broadcast a message to all clients. | ![server](https://img.shields.io/badge/Server-green) |
| [networkStats](#networkstats) | Report network traffic stats. | ![server](https://img.shields.io/badge/Server-green) |
| [passvote](#passvote) | pass a vote. | ![server](https://img.shields.io/badge/Server-green) |
| [RemoveGuidFromBanList](#removeguidfrombanlist) | Removes a GUID from the banlist. | ![server](https://img.shields.io/badge/Server-green) |
| [RemoveIPFromBanList](#removeipfrombanlist) | Removes an IP from the banlist. | ![server](https://img.shields.io/badge/Server-green) |
| [ShowBanList](#showbanlist) | Displays the banlist. | ![server](https://img.shields.io/badge/Server-green) |
