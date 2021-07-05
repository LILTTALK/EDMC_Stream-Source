# [Elite Dangerous Market Connector](https://github.com/Marginal/EDMarketConnector/wiki) - Stream Source

This plugin outputs status info from the game Elite Dangerous to files for use as text sources in live streaming software such as Open Broadcaster Software, GameShow, XSplit, etc. It outputs status info from the game [Elite Dangerous](https://www.elitedangerous.com/) to files for use as [text sources](https://obsproject.com/wiki/Sources-Guide#text-gdi) in live streaming software such as [Open Broadcaster Software](https://obsproject.com/), [GameShow](http://gameshow.net/), [XSplit](https://www.xsplit.com/), etc. 

## Installation

This plugin works currently with EDMC version 5.x.x. All previous versions of EDMC will cause errors in the output files.

* On EDMC's Plugins settings tab press the “Open” button. This reveals the `plugins` folder where EDMC looks for plugins.
* Download the [latest release](https://github.com/LILTTALK/EDMC_Stream-Source/releases/latest).
* Open the `.zip` archive that you downloaded and move the `EDMC_Stream-Source` folder contained inside into the `plugins` folder.

You will need to re-start EDMC for it to notice the new plugin.

## Output

The plugin writes the following status files into the folder that you specify in EDMC's Output settings tab:

* `EDMC System.txt` - Name or the current star system.
* `EDMC StarPos.txt` - Star system's galactic coordinates.
* `EDMC Station.txt` - Name of the planetary or space station at which the player is docked. Empty if not docked.
* `EDMC Body.txt` - Name of the nearby star, planet or ring. Empty if not near any celestial body.
* `EDMC LatLon.txt` - Latitude and longitude coordinates. Empty if not near a planet.
* `EDMC Station or Body.txt` - Name of the station if docked, otherwise the name of the nearby celestial body, or empty.
* `EDMC Station or Body or System.txt` - Name of the station if docked, otherwise the name of the nearby celestial body, otherwise the name of the star system.
* `EDMC ShipType.txt` - Ship type, e.g. Krait Phantom.
* `EDMC ShipName.txt` - Ship name, if the ship has been named. Otherwise ship type.

If the app is started while the game is not running these files hold placeholder values, which can be used to position the text in OBS Studio and other streaming software.

## Credits

Jonathan Harris (Original Creator)

## License
Everyone is permitted to copy and distribute verbatim copies of this license document. 
