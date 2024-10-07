<h1>Strategy Game Troops</h1>
 
 ### [YouTube Demonstration](https://www.youtube.com/watch?v=f-oodmdnpl0)

<h2>Description</h2>
Project consists of a Troop scriptable object with a custom editor that allows for easy editing, and creation. These Troop scriptable objects are then used in the TroopSpawner to be spawned with random names and color combinations predetermined in the Troop scriptable object. For simplicity the TroopSpawner also moves the Troops when receiving input from the TroopController.
<br/>

<h2>Languages and Enviroments</h2>

- Unity
- C#
- Windows 10
- Visual Studio Code

<h2>Libraries</h2>

- Unity Engine
- Unity Editor
- System.Collections
- System.Collections.Generic

<h2>System Walkthrough:</h2>
<p align="center">
Create a new troop using the create menu: <br/>
<img src="https://i.imgur.com/UleuUU8.png" height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Add the TroopType enum: <br/>
<img src="https://i.imgur.com/rKWsyLD.png" height="30%" width="30%" alt="Object Spawner Steps"/>
<br />
<br />
Fill out the troop details: <br/>
<img src="https://i.imgur.com/jE9vboV.png" height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Add the TroopSpawner to your spawner gameobject: <br/>
<img src="https://i.imgur.com/jEYsFvp.png" height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Populate the troops to spawn list, only the first 5 (0-4) will be able to be spawned: <br/>
<img src=https://i.imgur.com/RAUkuW0.png height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Adjust the position and spawn size of the spawner, gizmos in the scene will show the spawn area: <br/>
<img src=https://i.imgur.com/2DUNOQw.png height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Add the TroopController script to your player gameobject and reference the TroopSpawner: <br/>
<img src=https://i.imgur.com/cowY2PQ.png height="60%" width="60%" alt="Object Spawner Steps"/>
<br />
<br />
Press play and select your troop by using the number keys(0-5), this corresponds to the first 5 troops in your TroopSpawner. 
<br/>After selecting your troop press TAB to spawn the troop: <br/>
<img src=https://i.imgur.com/BLCLOBh.png height="90%" width="90%" alt="Object Spawner Steps"/>
<br />
<br />
Left clicking will teleport all selected spawned troops to your cursor if it can find a valid position: <br/>
<img src=https://i.imgur.com/Kjpg7oq.png height="70%" width="70%" alt="Object Spawner Steps"/>
<br />
<br />
Otherwise if you click on a invalid position the troops will just teleport to 0, 0, 0 for demostration purposes: <br/>
<img src=https://i.imgur.com/bHKULuK.png height="70%" width="70%" alt="Object Spawner Steps"/>
<br />
<br />
Each troop will be named and colored. Each unique name gets assigned a color, and every subsequent troop with the same name with get appended with the number of times this name has been used: <br/>
<img src=https://i.imgur.com/7186mbN.png height="90%" width="90%" alt="Object Spawner Steps"/>
<br />
<br />
The console will display what color corresponds to what name, how many units were spawned when spawning a troop, and when the spawn cooldown is active: <br/>
<img src=https://i.imgur.com/ba9mvCI.png height="70%" width="70%" alt="Object Spawner Steps"/>
