Spawns all new characters in a designated lobby cell. Can be used to present different starting location choices, staring equipment or other server related activities. Players can not die inside the cell (optional).  
You will need some way to connect that cell to the rest of the world, one such is my [DoorFramework](https://github.com/tes3mp-scripts/DoorFramework).  
Comes with an optional permadeath module, that doesn't let dead players leave the lobby (require `permadeath.lua` similarly to how you enable `main.lua` to enable).

Requires [DataManager](https://github.com/tes3mp-scripts/DataManager)!

You can find the configuration file in `server/data/custom/__config_PlayerLobby.json`.
* `cell` cellDescription of your chosen lobby cell. I recommend one of the [test cells](https://en.uesp.net/wiki/Morrowind:Test_Cells).
* `pos` position in which to spawn players inside given cell.
* `rot` initial rotation of players spawning in.
* `invulnerability` whether player should not be able to die inside the lobby cell.

Provides a `PlayerLobby_Leave` event and a `teleportToLobby(pid)` function to be used in other scripts.