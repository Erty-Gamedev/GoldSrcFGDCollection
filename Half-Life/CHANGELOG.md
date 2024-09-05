# Half-Life FGD Changelog

## v1.0.0
Initial version based on the Goldsorce Games FGD Collection as retrieved from
[TWHL's Tools and Resources](https://twhl.info/wiki/page/Tools_and_Resources#Game_Data_Files)
page on 2024-08-29.
This version was referred to as "3.0.0.1" in the original file, and will be
known as v1.0.0 in this project.

Changelog retrieved from comment field of this file:

> aug 28 2001 - 3.0.0.1
> - changed IS NOT LOOPED to NOT TOGGLED on ambient_generic (royalef)
> - gave light_environment a Name
> - added Angular Velocity to func_train
> - added cycler_wreckage (Waldo)
> - created ZHLT_point baseclass
> - added ZHLT_point base to light, light_environment, and light_spot
> - created ZHLT baseclass
> - added ZHLT base to all applicable brush entities
> - above list compiled by Unquenque


## v1.1.0
Major refactor started by Erty.

* Extract rendermode/fx/amount/color into baseclasses and added missing 18 and 19 Render FX choices
* Renamed monster_satchelcharge to monster_satchel
* Added additional ZHLT keyvalues from VHLT
* Added missing keyvalues to entities
  - `health` removed from func_door[_rotating] (non-functional left-over from Quake)
  - `healthvalue` to func_door[_rotating] (gives this amount of health to activator when opened)
  - `zhlt_usemodel`, `zhlt_copylight` and `light_origin` to common (solid and point) ZHLT base class
  - `zhlt_noclip`, `zhlt_invisible`, `zhlt_customshadow`, `zhlt_embedlightmap` `zhlt_embedlightmapresolution` and `_minlight` to solid entity ZHLT base class
  - `zhlt_stylecoring` added to light and light_spot (controls black threshold for styled/named lights)
  - `killtarget`, `target` and `message` to entities that use these, removed from entities that don't
* Added studio() parameters to ammo, items, weapons, monsters, etc
* Added `body` and `skin` keys to monster, ammo, item, and weapon entities, as well as to cycler
* Changed many Target key types to target_destination (was incorrect type target_source)
* Updated descriptive names of various keys to be more explanatory
* Renamed beverage types to correspond better with can.mdl skins
* Changed default values of certain entities
  - func_illusionary now has `zhlt_noclip = 1`
  - trigger_relay and trigger_auto now has `triggerstate = 2` (TOGGLE) instead of `0` (OFF)
  - light_environment now has `pitch = -90` (sun directly overhead)
* Various cleanups of formatting and structure of FGD, to make it more tidy and organized
