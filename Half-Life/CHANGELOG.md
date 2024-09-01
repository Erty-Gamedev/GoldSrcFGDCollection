# Half-Life FGD Changelog

## v1.0.0
Initial version based on the Goldsorce Games FGD Collection as retrieved from
[TWHL's Tools and Resources](https://twhl.info/wiki/page/Tools_and_Resources#Game_Data_Files)
page on 2024-08-29.
This version was referred to as "3.0.0.1" in the original file, and will be
known as v1.0.0 in this project.

Changelog retrieved from comment field of this file:

aug 28 2001 - 3.0.0.1
- changed IS NOT LOOPED to NOT TOGGLED on ambient_generic (royalef)
- gave light_environment a Name
- added Angular Velocity to func_train
- added cycler_wreckage (Waldo)
- created ZHLT_point baseclass
- added ZHLT_point base to light, light_environment, and light_spot
- created ZHLT baseclass
- added ZHLT base to all applicable brush entities
- above list compiled by Unquenque


## v1.1.0
Major refactor started by Erty.

* Extract rendermode/fx/amount/color into baseclasses
* Renamed monster_satchelcharge to monster_satchel
* Added additional ZHLT keyvalues from VHLT
* Added studio() parameters to ammo, items, weapons, monsters, etc
* Changed many Target key types to target_destination (was incorrect type target_source)
* Renamed beverage types to correspond better with can.mdl skins
