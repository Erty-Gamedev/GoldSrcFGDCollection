# Day of Defeat FGD Changelog

## v1.0.0
Initial version based on the Goldsorce Games FGD Collection as retrieved from
[TWHL's Tools and Resources](https://twhl.info/wiki/page/Tools_and_Resources#Game_Data_Files)
page on 2024-08-29.
This version was referred to as "2.0.3.A.SP" in the original file, and will be
known as v1.0.0 in this project.

Changelog retrieved from comment field of this file:

> ### Revision history
> 
> by Justin DeJong aka "N0TH1NG"
> modified from code by Chris Bokitch aka "autolycus"
> by Tim Holt aka Waldo (burkenholt@home.com)
> modified from code by Justin DeJong aka "N0TH1NG"
> Version 0.7.3 and 0.7.4 by Morlam (morlam@gamespotmail.com)
> slightly modified from code by Chris Bokitch (Autolycus), Justin DeJong (NOTH1NG), and
> Tim Holt (Waldo).
> 
> version 0.8.0 by Matt Boone aka "Mugsy"
> modified from version 0.7.4
> version 2.0.1 by Tim Holt aka "Waldo"
> modified from version 0.8.0 
> changed first digit of version number to reflect DoD version.
> version 2.0.2 by Brandon Russell aka "Axis"
> modified from version 2.0.1
>
> ---
>
> #### Original changes by Tim Holt (0.7.0)
>
> - Added new Trigger Changetarget sprite (green cube w/words)
> - Added new Info Target sprite (bullseye)
> - Added new trigger_camera sprite (Video camera)
> - Added new Multi Manager sprite (box w/arrows coming out of it)
> - Added new "Cycler Sprite" sprite (box w/arrow circle around it)
> - Added replacement ambient_generic sprite (changed from speaker to speaker with words "Ambient Generic" > around it")
> - Added replacement env_sound sprite (changed from speaker to speaker with words "Env Sound" around it")
> - Added replacement light_spot sprite (changed from lightbulb to spotlight)
> - Added replacement Light Environment sprite (changed from lightbulb to sun)
> - Added all the "game_*" entities
> - Added info_compile_params and info_lights_rad entities.  Idea is to get someone like Zoner to > implement support for them in Zoners, or build support for them into a compile tool like Q2Beaver, HLCC, > etc.
> - Added env_funnel
> - Added trigger_gravity
> - Added player_weaponstrip
> - Put Zoners RAD option (that allow solid (func_) based ents to cast shadows) into a number of new additional items that can support it. Use with caution, as for example a func_pushable can cast a shadow now, but if you push it, the shadow stays behind :^)
>
> #### 12/31/2000 - Tim Holt (0.7.1)
>
> - Added new sprites for all the Game entities
> - Added new sprite for Player Weapon Strip
> - Added new sprite for Trigger_Relay
> - Added new sprite for Trigger_ChangeTarget
>
> #### 01/01/2001 - Tim Holt (0.7.2)
>
> - Added new dropdown to hostage entity, so you can choose hostage skin directly by name (orange suit guy or tie guy)
> - Removed commented out "master" option for game_zone_player.  It was commented out from the original HL FGD for some reason.  Not sure why or if maybe there is a problem with it?
>
> #### 01/04/2001 - Morlam (0.7.3)
>
> - Arranged all the point entities in alphabetical order
> - Corrected a typo in hostage_entity: "Orange Suit Worker" from "Orange Suite Worker".
> - Changed func_water default WaveHeight to 0
> - Added ZHLT Light Flags to func_plat, _pendulum and _vehicle
> - Under info_compile_params:
>	- Changed extra to choices instead of a string; default is now 0
>	- Changed extra to read: "Enable Extra mode in HLRAD?"
>	- Added hullfile, chop, texchop, circus, and dscale keys
>	- Added "No Clip" flag under Run BSP in the spawnflags
> - Under info_lights_rad:
>	- added radfile key/value, specifies custom texture light file
>
> #### 01/05/2001 - Morlam (0.7.4)
>
> - Added _fade and _falloff keys to the light_ entities.  Need ZHLT 2.2+ for these to work.
> - Added light_origin key to the ZHLT Light Flags BaseClass.  Again, you need the latest version of Zoner's Tools for light_origin to work.
> - Moved circus and extra from the "Class Info" tab to the "Flags" tab.
> - Shortened the SmartEdit names of certain key/values in info_compile_params so that they aren't cut off (at least, on my 800X600 screen on a 15 inch monitor).
Jan 6, 2001 - Tim Holt (0.7.5)
> - Added new parameter options for game_player_equip to list all CS items in dialog, thus removing the need to turn off SmartEdit to configure.
> - Added new sprite for trigger_auto (green box with words "Trigger Auto")
>
> #### Jan 26, 2001 - Tim Holt (0.7.6)
>
> - Added "No Clients" check option to Trigger base class per suggestion/lead from Mataleone (cs mapping forum)
>
> #### Aug 27, 2001 - Tim Holt (0.7.7)
>
> - Removed some old CS entities that had not been removed
> - Added cycler_wreckage
> - Added Angular velocity option to func_train (see http://www.chatbear.com/cgi-bin/board.pl?action=viewthread&threadid=252,994640145,10305&id=47702&rdid=9)
>
> #### Dec, 2001 - Matt Boone ( 0.8.0 )
> - added dod 2.0 objectives
>
> #### Dec 11, 2001 - Tim Holt (2.0.0bmp)
>
> - merged some spirit features with Matt Boone's revised 2.0 DoD entities
>
> #### Jan 11, 2002 - Brandon Russell (2.0.2bmp)
>
> - Added 2 new settings to the spawn flags of Game_text to fix Kami's map
>
> #### April 26, 2002 - Tim Holt (2.0.3mp)
> Rolling in a bunch of fixes based 
> - Removed info_initial_player_allies as it is no longer used in 2.0
> - Removed info_initial_player_axis as it is no longer used in 2.0
> - Removed sprite from info_player_allies and info_player_axis. Hard to judge player spawn location and player size with sprites. Axis is red, Allies are green. Colors were also incorrect for these entities.  Set to be correct.
> - Added new _defuse_light attribute for the HLRAD tweak by Adam Foster (see http://www.chatbear.com/cgi-bin/board.pl?action=viewthread&threadid=860,1014492782,1883&id=158865&rdid=653&view=flatold 
> - Added missing "movewith" attribute to all trigger brush ents
> - Added skin value -3 for water to func_illusionary
> - Added in all the weapon_ entities for weapons on the ground
> - Added in all the ammo_ entities for ammo on the ground
>
> #### April 28, 2002 - Tim Holt (2.0.3.A.SP)
>
> Adding in single player stuff
> - Add HintTypeChoices base class
> - Add ActivityTypeChoices base class
> - Add Monster base class
> - Add info_node entity
> - Add info_intermission entity
> - Add info_landmark entity
> - Add AiScriptedSequence entity
> - Added scripted_action entity
> - Added scripted_sentence entity
> - Added scripted_sequence entity
> - Added trigger_transition entity
> - Added monster_axis_grunt
> - Added monster_allied_grunt
> - Added monster_allied_barney

## v1.1.0
Originally named version 4.0 and committed by Yui.
Comment field changelog was removed but preserved in a re-formatted form [above](#v100).
No formal changelog was given, however here is a summary based on a diff comparison:

* Entity property changes:
  - `cam_fade` added to DoDCam base class
  - `m_iClass` added to BaseTank base class
  - `master` and `hintmsg` to env_message, as well as added more spawnflags:
    - *Allies Only* (4)
    - *Axis Only* (8)
    - *Allied Player Only* (16)
    - *Axis Player Only* (32)
  - Added *Ignore Allies* (1) and *Ignore Axis* (2) spawnflags to game_zone_player
  - Removed *Trigger at every round start* (512) spawnflag from trigger_auto
  - Removed *Reset at round restart* (1) from trigger_multiple and trigger_once
  - `capobj_group`, `tnttrigger`, `tntdelay` and `capobj_hud_sprite` added to func_breakable, as well as the following spawnflags:
    - *Only Grenades* (8)
    - *Allies Only* (16)
    - *Axis Only* (32)
    - *Object Cap Only* (64)
    - *Bazooka or Grenades* (256)
    - *Only Bazooka* (512)
  - `m_iDamage` added to func_mortar_field
  - *Not Interruptible* (16) spawnflag added to func_train
* Added `studio()` parameter to env_model
* Added new entities:
  - info_intermission
  - dod_preround
  - particle_shooter
  - info_landmark
  - scripted_action
  - scripted_sentence
  - scripted_sequence
  - trigger_transition
  - monster_axis_grunt
  - monster_allied_grunt
  - monster_allied_barney

> [!NOTE]
> Some of the above changes are referred to in the [v1.0.0 (2.0.3.A.SP)](#v100)
> comment field changelog, despite missing from that version's FGD.
> I'm unsure why this was done, or if there's any relation.

## v1.1.1 Patch

Originally named version 4.1, this patch adds in game_player_equip entity.
Yui added in this change that was published by [iNodeuNode on Reddit](https://www.reddit.com/r/DayOfDefeat/comments/ufrt0q/updated_dodfgd_to_v41_added_game_player_equip/).
