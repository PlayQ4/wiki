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
| callvote |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| cancelcoach |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| coach |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| coachdecline |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| coachinvite |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| coachrevoke |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| demoSlowDown |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| demoSpeedReset |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| demoSpeedUp |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| fixUserInfo |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
| follow |   |   |   | ![client](https://img.shields.io/badge/Client-blue) |
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
| addBot |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| AddGuidToBanList |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| AddIPToBanList |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| broadcastMsg |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| networkStats |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| passvote |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| RemoveGuidFromBanList |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| RemoveIPFromBanList |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
| ShowBanList |   |   |   | ![server](https://img.shields.io/badge/Server-green) |
