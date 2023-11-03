# ChunkLoader

You can build an observation column. The area of one chunk around it will always be active. If you don't know what chunks are, you can press [Shift + E] on the column and the workspace will be highlighted.

It can be useful for breeding animals or farm mobs. You will put a column next to it and you can safely go do anything else, and the wolves will continue to multiply and the mobs will die. You can also configure the column limit per player in the configuration.

The column must be charged like a torch. By default, a thunderstone. In the absence of recharge, the column will turn off and stop working. If desired, in the configuration of the mod, you can remove the need for charging or change the necessary item.

The configuration is synchronized with the server.<br>
Config:
```
[Fuelling]

# Setting type: Int32
# Default value: 100
Max fuel = 100

# Setting type: Int32
# Default value: 1
Start fuel = 1

# Setting type: String
# Default value: Thunderstone
Fuel item = Thunderstone

# Setting type: Int32
# Default value: 5
Minutes for one fuel item = 5

# Setting type: Boolean
# Default value: false
Infinite fuel = false

[General]

# Setting type: Toggle
# Default value: On
# Acceptable values: Off, On
ServerConfigLock = On

[Main]

# Setting type: Int32
# Default value: 2
ChunkLoaders limit by player = 2

# Setting type: Color
# Default value: FFEB04FF
Terrain flash color = FFEB04FF
```

### <ins>If something does not work for you, you have found any bugs, there are any suggestions, then be sure to write to me!</ins>
 
Discord ```justafrogger```<br>
If you need a custom mod, do not hesitate to write 😉.
