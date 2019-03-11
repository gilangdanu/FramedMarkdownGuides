
# Revert Game Update using Steam Console

### 1. Install or open Steam Console
Install steamcmd.exe from [here](https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip) and login to your Steam account.
Alternatively, you can access Steam console from client or internet browser by typing `steam://nav/console`
or adding `-console` on Steam target address shortcut. 

### 2. Look up the game you want to revert the update 
Go to http://www.steamdb.info and type the name of the game into search bar on top left.

### 3. Get AppID. 
After searching the name of the game, record its appID.

### 4. Get DepotID.
After that, you need to find the content you want to download by take a look at depot list. The easiest way to find the depot you need is by comparing files on SteamDB with your local files, if they're identical, that's most likely the depot you want to download. Record its DepotID.

Example:
![depot example](\Images\steamcmd-guide-1.jpg)

### 5. Get ManifestID
Every specific version of the content you want to download are listed on 'Manifests' tab. They're marked by timestamp and ManifestID. Record the ManifestID

### 6. Download the package
Once you have AppID, DepotID and ManifestID type this into Steam console 
`download_depot <appid> <depotid> <manifestid>`

### 7. Retrieve the package
If you're installing SteamCMD somewhere in your PC, the downloaded package will be on the same folder as your steamcmd.exe. If you're opening Steam Console via client or browser, the downloaded package will be on this folder
`\Steam\steamapps\content\<depotid number>`

### 8. Overwrite the new files with old one
After that, it's just a matter of replacing new, updated game files with the older one you just downloaded.