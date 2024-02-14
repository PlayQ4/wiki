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

**todo**
- aviNetDemo - Capture screenshots from a netdemo suitable for creating an avi.
- callvote - Provides a way to vote for many votable options.
- cancelcoach - Makes you quit your coaching position.
- coach - Accepts a coaching invitation.
- coachdecline - Declines a coaching invitation.
- coachinvite - Invites a player to coach your team.
- coachrevoke - Revokes a coach.
- demoSlowDown - Slow down netdemo playback.
- demoSpeedReset - Reset netdemo playback to normal speed.
- demoSpeedUp - Speedup netdemo playback.
- fixUserInfo - Attempts to get your userInfo from the server.
- follow - Allows a spectator to switch to a nominated player when spectating.
- lockteam - Locks/unlocks your team from players.
- maplist - Lists all the maps available on the server.
- multipov - Allows a spectator to view all members of a team at once.
- networkStats - Report network traffic stats.
- players - Lists all players, and a unique player id to use with other commands.
- referee - Used to make yourself a referee, granting limited admin rights.
- reloadHud - Reloads the current hud.
- specinvite - Invites a player to spectate your team.
- speclock - Locks/unlocks your team from spectators.
- specrevoke - Revokes an invited spectator of your team.
- teamready - Marks everyone on your team as ready.
- timeout - Calls a timeout - a limited version of pause for non-referees.
- timein - Calls the end of a timeout.
- viewSizeDown - Decrease view size.
- viewSizeUp - Increase view size.
- weapon - Switches to the given weapon - an alias of _impulseX.

### Referee commands

| Command | Parameters | Summary | Description | Type |
| --- | --- | --- | --- | --- |
| abort |  | Abandons the current game and returns to warmup. | This command is intended to be used when a match needs to be abandoned. It sets all players to "not ready", and resets the game back to the warmup. | ![referee](https://img.shields.io/badge/Referee-orange) |
| allready |   | Readies up all players and begins the game. | This forces all players to be "ready", even if they have not readied up themselves, thus allowing the game to begin. | ![referee](https://img.shields.io/badge/Referee-orange) |

**todo**
- cancelref - Makes you quit your referee position.
- coachMarine - Assigns a given player to coach duty for the marine team.
- coachStrogg - Assigns a given player to coach duty for the strogg team.
- ingame - Puts a given player in a non-team game.
- lockteams - Locks teams to prevent players joining mid-game.
- marine - Puts a given player on the marine team.
- pause - Pauses a game.
- remove - Removes a given player from a game.
- specBoth - Turns a given player into an all-seeing spectator.
- speclockall - Locks both teams from spectators.
- speclockmarine - Locks the Marine team from spectators.
- speclockstrogg - Locks the Strogg team from spectators.
- specMarine - Turns a given player into a marine spectator.
- specStrogg - Turns a given player into a strogg spectator.
- specunlockall - Unlocks both teams from spectators.
- specunlockmarine - Unlocks the Marine team from spectators.
- specunlockstrogg - Unlocks the Strogg team from spectators.
- strogg - Puts a given player on the strogg team.
- unpause - Unpauses a game.
- unlockteams - Unlocks teams to allow players to join.

### Server commands


| Command | Parameters | Summary | Description | Type |
| --- | --- | --- | --- | --- |
| AddGuidToBanList | \<GUID\> | Adds a GUID into the banlist. | Adds the given GUID into the banlist. The guid is a q4 guid, as shown by the players command. Another useful source of of player to GUID mappings is from the stats XML logs. If the guid contains non-alpha chars, it is worth quoting the parameter to make sure it is entered correctly. | ![server](https://img.shields.io/badge/Server-green) |
| AddIpToBanList | \<IP\> | Adds an IP into the banlist. | Adds the IP into the banlist. If the ip is just the beginning of the IP (eg 123.123.123) then it will ban 123.123.123.* - do not use wildcards though, its automatic. Note that you must use the IP as displayed in the q4 console at connection - this is usually dotted quads, but it is sometimes resolved in the case of localhost, and maybe other computers on the sam LAN. | ![server](https://img.shields.io/badge/Server-green) |
| addBot | \<name\> \<team\> | Add a bot. | Add a "name" bot. If the name matches a defined bot personality, the defined bot will be added, otherwise it will be a default bot. In team games, you can also specify the team (strogg or marine, marine if unspecified). | ![server](https://img.shields.io/badge/Server-green) |

**todo**
- broadcastMsg - Broadcast a message to all clients.
- networkStats - Report network traffic stats.
- passvote - Pass a vote.
- RemoveGuidFromBanList - Removes a GUID from the banlist.
- RemoveIPFromBanList - Removes an IP from the banlist.
- ShowBanList - Displays the banlist.
