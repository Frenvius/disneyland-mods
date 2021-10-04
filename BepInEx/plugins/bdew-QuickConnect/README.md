# Quick Connect mod for Valheim

Adds a quick connect window with a configurable list of servers, no more dealing with steam's buggy favorites widow and entering passwords (twice).  
  
**Installation**  
1.  [Install BepInEx](https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/) following the instructions at the link.
      If you have Valheim Plus, you can skip that step as it already includes it with the download.
3.  Extract he zip file into your BepInEx folder
4.  Edit quick_connect_servers.cfg in BepInEx/config folder to add your servers
5.  Run the game and press connect button on title screen

  Config file has a list of servers in the following format:  
  
```
name:addr:port[:password]
```
**addr** can be ether IP or a fully qualified domain name .
**password** is optional, you can skip it if your server doesn't need a password or if you don't want to write it down.
  
**Example config:**  
 ```
Awesome Server:127.0.0.1:2456:smellysocks
```

## License

This mod is free software: you can redistribute it and/or modify it under the terms of the [GNU Lesser General Public License](http://www.gnu.org/licenses/lgpl-3.0.en.html) as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

