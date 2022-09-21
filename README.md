# [NMRiH] NMRiH Diffmoder fork     
**Sourcemod plugin which allows changing of gamemode via voting.**

For base information about the plugin go here:
*https://forums.alliedmods.net/showthread.php?t=301322*

This fork includes some changes and features to the original, such as:

- Automatically reverts back to the default gamemode after the server has been empty for a while. This may be set with the nmrih_autodefault_timer ConVar
- Runner mod now uses the game's built in BecomeRunner() function using a vscript function. This method prevents nmrih zombie spawn brushes from completely stopping spawning.
- A new mode to play: Anklebiters, which converts all zombies into speedy crawlers.
- The option to toggle double jump; requires Double Jump (1.0.1) by Paegus (_https://forums.alliedmods.net/showthread.php?p=895212_)

## Requires DHooks:
https://forums.alliedmods.net/showthread.php?t=180114


## Cvars:
- sv_current_diffmode                 -   Info about the current diffmode.           default:  0
- g_cfg_doublejump_enabled            -   Double Jump:       0 disabled, 1 enabled.  default:  0
- nmrih_diffmoder                     -   Enable/Disable plugin.                     default:  1
- nmrih_diffmoder_infinity_default    -   Infinity ammo on?  0 No, 1 Infinite ammo, 2 Infinite clip.             default:  0  
- nmrih_diffmoder_gamemode_default    -   Default gamemod,   0 Shamblers, 1 All runners, 2 All kids, 3 Crawlers. default:  0
- nmrih_diffmoder_friendly_default    -   Friendly fire:     0 off, 1 on             default:  0 
- nmrih_diffmoder_realism_default     -   Realism:           0 off, 1 on             default:  0
- nmrih_diffmoder_hardcore_default    -   Hardcore survival: 0 off, 1 on             default:  0
- nmrih_diffmoder_difficulty_default  -   Default difficulty: classic, casual, nightmare                 default:  "classic"
- nmrih_diffmoder_casual_cooldown     -   Casual switch cooldown time.                                   default:  300
- nmrih_autodefault_timer             -   Time in seconds until diffmoder reverts to default gamemode.   default:  1200
- nmrih_diffmoder_mapchange_default   -   Change the diffmode to default after map change. 0: off, 1: on.default:  1

<pre>
Feel free to use the code or plugin in any way

Credits:

Mostten - [NMRiH] Difficulty and Mod changer(zombies convert to all runners)  - Original diffmoder plugin
Ryan    - [NMRiH] Zombie Speeds (v1.6, 2020-04-06)                            - speed manip snippets
Dysphie - [NMRiH] Backpack 2                                                  - Vscript Proxy, and giving the idea of using it
</pre>
