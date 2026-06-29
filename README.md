# 2008M Roblox patch guide
**⚠️ PLEASE DO NOT USE THIS FOR MULTIPLAYER OR PUBLIC REVIVALS THIS IS VERY UNSECUREABLE ⚠️**

_This patching guide patches:_

- [x] Trust check (load any asset from any internet resource) (unsecureable stars: ⭐⭐⭐⭐⭐)
- [x] Player name anti-change bypass (unsecureable stars: ⭐⭐)
- [ ] Another patches lol

This also patches 2007, 2009 and others (I am not checked) so LOL

_Tools you need to patch:_

- x32dbg
- your brain

**1. Trust check bypass**
(This is very unsecureable so any cheater on the server can execute script and load ANY virus model to server)

1. Open x32dbg
2. Open Roblox executable
3. Go to "Symbols"
4. In the left list double left click on the Roblox executable name
5. Click "A2" button in the upper panel
6. Wait until loads then find in bottom textbox "trust check"
7. You find 2 variables of "trust check failed", go to upper
8. Go up before you not found line that starts from "jne"
9. Select this line and press space on your keyboard
10. Replace the "jnz" to "jmp" (Do not touch other values in the right!) then save
11. Go back to references and do it again with bottom "trust check failed".
12. Done.

**2. Set As Player name bypass**
(This unsecureable because any guy on server can play as your name and id)

1. Open x32dbg (if already not)
2. Open Roblox executable (if already not)
3. Go to "Symbols"
4. In the left list double left click on the Roblox executable name
5. Click "A2" button in the upper panel
6. Wait until loads then find in bottom textbox "set as Player's name"
7. You find 2 variables of "set as Player's name", go to upper
8. Find "push 3" under the line bottom
9. Select this line and press space on your keyboard
10. Change 0x03 (or 0x3) to 0x0
11. Go back to references and do it again with bottom "set as Player's name".
12. Done.

# Playing
Load any map, go to command and paste commands in turn:

`game.Players:CreateLocalPlayer(0)`,
`game.Players.LocalPlayer.Name = "Test" --Your name here`,
`game.Players.LocalPlayer:LoadCharacter()`,
`game:GetService("RunService"):Run()`

**Done! Have fun!**
