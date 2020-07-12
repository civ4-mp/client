# Civilization 4 Multiplayer

The multiplayer mode of Civilization 4 used the GameSpy servers that were shut down in 2014.
Since then, the community develops and hosts alternative servers to keep Civilization 4 multiplayer alive.

### Pitboss

The Pitboss mode, or any other direct-ip connection, in Civilization uses a NAT negotiation server (natneg) to help connections when multiple players join the same game.

### Lobby

The Multiplayer lobby provides services for login, chat and game browser. It also uses the natneg for games with more than two players.

## How to use the community servers

In order to use the community servers, you have to tell your game to connect to them.
Since they are not normally configurable, there are two alternatives.

### A) Use a patched exe file

Download one of these files and run

#### Beyond The Sword (BTS)
https://github.com/civ4-mp/client/raw/master/Civ4BeyondSword2015.exe

#### Base Game (vanilla)
https://github.com/civ4-mp/client/raw/master/Civilization4_2015.exe

The files only change the hardcoded domain names for the multiplayer servers. This is the *easiest* way and it will work in the future as long as Zulan hosts the natneg/lobby server on his domain.

### B) Modify the `hosts` file

Modify your `hosts` file to include the following contents https://github.com/civ4-mp/client/raw/master/hosts .
The file is located at `C:\Windows\System32\drivers\etc\hosts` on windows and `/etc/hosts` on Linux. You need to use an editor with administator permissions to edit the file.

This is the *safest* way. However, you may need to update some time in the future if the IP address of the server changes.
