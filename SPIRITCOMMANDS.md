# Full list of commands available to GMs

## About
**Date of Creation:** 19/8/2020  
**Date last Updated:** 13/12/2021  

**Author:** KOOKIIE  
**Maintained by:** KOOKIIE  

Note on account types, and their level of access:  

Enum Types | Value | Value (hex) | Value (bin) 
:--- | ---: | ---: | ---:
[**Player**](https://github.com/KOOKIIEStudios/SpiritSuite/blob/main/SPIRITCOMMANDS.md#player-level-commands) | 0 | 0x00 | 0b00000000
[**Tester**](https://github.com/KOOKIIEStudios/SpiritSuite/blob/main/SPIRITCOMMANDS.md#tester-level-commands) | 32 | 0x20 | 0b00100000
[**Intern**](https://github.com/KOOKIIEStudios/SpiritSuite/blob/main/SPIRITCOMMANDS.md#intern-level-commands) | 8 | 0x08 | 0b00001000
[**GameMaster**](https://github.com/KOOKIIEStudios/SpiritSuite/blob/main/SPIRITCOMMANDS.md#gamemaster-level-commands) | 16 | 0x10 | 0b00010000
[**Admin**](https://github.com/KOOKIIEStudios/SpiritSuite/blob/main/SPIRITCOMMANDS.md#admin-level-commands) | 16 | 0x10 | 0b00010000

Most of the commands are inheritted from Swordie - those that are have been labelled as `Inherited from Swordie`.  
Do note that these may differ from Swordie's logic/arguments, due to changes made by Team SPIRIT.  
Those without the label are only applicable to SpiritMS.

### PLEASE CREDIT THE AUTHOR IF YOU USE/QUOTE THIS DOCUMENT ELSEWHERE

## Player level commands:

NOTE: Regular player commands (which use the `@` prefix instead of `!`) are excluded from this list.

**!map**\
Inherited from Swordie. Level: **Player**
>Prints a System Notice of all characters in the user’s map

## Tester level commands:

**!showinvinfo**\
**!invinfo**\
Inherited from Swordie. Level: **Tester**
>Prints out the name, generic item ID, specific item ID, bag index, and inventory type, for every item in inventory, in the user’s chatbox. (Presumably for debug purposes)

\
**!checkid**\
**!getid**\
**!charid**\
Inherited from Swordie. Level: **Tester**
>Prints out the user’s character ID and account ID, in the user’s chatbox. (Presumably for debug purposes)

\
**!getphantomstolenskills**\
Inherited from Swordie. Level: **Tester**
>Prints out skills the user has stolen as a Phantom, in the user’s chatbox. (Presumably for debug purposes)

\
**!stealskilllist**\
Inherited from Swordie. Level: **Tester**
>Display skill list (containing every stealable-skill) to steal from. (Presumably for debug purposes)

\
**!np**\
**!nearestportal**\
Inherited from Swordie. Level: **Tester**
>Prints out map and portal information (within 30 pixels) for the map the user is in, in the user’s chatbox. (Presumably for debug purposes)

\
**!stats**\
Inherited from Swordie. Level: **Tester**
>Prints out the user’s stats, in the user’s chatbox. (Presumably for debug purposes)

\
**!fame**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!fame** | **\<IGN\>** | **\<amount\>**
**!setfame** | **\<IGN\>** | **\<amount\>**
>Sets the fame of the target user to the specified value.

\
**!traitexp**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!traitexp** | **\<trait name\>** | **\<amount\>**
>Types: charm, diligence, willpower, insight, empathy, ambition (non-case sensitive)\
(Also valid: craft, will, sense, charisma)\
Increments the trait exp by the specified value.

\
**!testdrop**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |
:---|---|---
**!testdrop** | **\<mob ID\>** 
**!testdrop** | **\<mob ID\>** | **\<amount\>** 
>Spawns the specified number (optional, defaults to 1) of the specified mob (with 3 HP). (Presumably for debug purposes)

\
**!done**\
Inherited from Swordie. Level: **Tester**
>Sets level to 235, HP/MP to 250,000, stats to 32000

\
**!hypertp**\
Inherited from Swordie. Level: **Tester**
>Gives the user a Hyper Teleport Rock

\
**!job**\
**!setjob**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |
:---|---|---
**!job** | **\<ID\>** | 
**!setjob** | **\<ID\>** | 
**!job** | **\<ID\>** | **\<subjob\>** 
**!setjob** | **\<ID\>**| **\<subjob\>** 
**!job** | **\<name\>** | 
**!setjob** | **\<name\>** | 
>Set the user’s job to the job ID specified.

\
**!sp**\
**!setsp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!sp** | **\<amount\>** 
**!setsp** | **\<amount\>**
>Give the user the specified amount of free SP in the user’s highest level skill tab.

\
**!ap**\
**!setap**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!ap** | **\<amount\>**
**!setap** | **\<amount\>**
>Give the user the specified amount of free AP.

\
**!hp**\
**!sethp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!hp** | **\<amount\>**
**!sethp** | **\<amount\>**
>Set the user’s Max HP to the specified amount.

\
**!mp**\
**!setmp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!mp** | **\<amount\>**
**!setmp** | **\<amount\>**
>Set the user’s Max HP to the specified amount.

\
**!str**\
**!setstr**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!str** | **\<amount\>**
**!setstr** | **\<amount\>**
>Set the user’s STR to the specified amount.

\
**!dex**\
**!setdex**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!dex** | **\<amount\>**
**!setdex** | **\<amount\>**
>Set the user’s DEX to the specified amount.

\
**!int**\
**!setint**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!int** | **\<amount\>**
**!setint** | **\<amount\>**
>Set the user’s INT to the specified amount.

\
**!lukv**\
**!setluk**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!luk** | **\<amount\>**
**!setluk** | **\<amount\>**
>Set the user’s LUK to the specified amount.

\
**!resetstats**\
**!resetap**\
Level: **Tester**
>Resets STR, DEX, INT, LUK (and frees up the AP)

\
**!level**\
**!setlevel**\
**!lvl**\
**!lv**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!level** | **\<amount\>**
**!setlevel** | **\<amount\>**
**!lvl** | **\<amount\>**
**!lv** | **\<amount\>**
>Set the user’s Level to the specified amount. (Stats not changed)

\
**!leveluntil**\
**!levelupuntil**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!leveluntil** | **\<amount\>**
**!levelupuntil** | **\<amount\>**
>Recursively level the user up till to the specified amount. (Stats not changed)

\
**!heal**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!heal** | **\<amount\>**
>Revives/recovers the user’s HP and MP by the specified amount. (capped at Max HP/MP)

\
**!curhp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!curhp** | **\<amount\>**
>Sets the user’s current HP to the specified amount.

\
**!curmp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!curmp** | **\<amount\>**
>Sets the user’s current MP to the specified amount.

\
**!invincible**\
Inherited from Swordie. Level: **Tester**
>Toggles the user’s invincibility.

\
**!morph**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!morph** | **\<ID\>**
>Not entirely sure what this does, tbh. It sets the option value to the specified morph ID, and the option’s skill ID to Kaiser’s Final Trance, before pushing the buff via the TSM.

\
**!mount**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!mount** | **\<ID\>**
>See above (sets the option value to the specified mount ID), but it also sets the user to be riding.

\
**!testtempstat**\
Inherited from Swordie. Level: **Tester**
>No idea what this does. Does something to the stats of the mobs in the user’s map.

\
**!setmap**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!setmap** | **\<map ID\>**
>Warps the user to the specified map.

\
**!setportal**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!setportal** | **\<portal ID\>**
>Warps the user to the specified portal

\
**!getskill**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |  |
:---|---|---|---
**!getskill** | **\<skill ID** | **\<current level\>** | **\<max level\>**
>Gives the user the specified skill with the specified current and max levels.

\
**!maxskills**\
Inherited from Swordie. Level: **Tester**
>Max all skills' levels in every tab.

\
**!lookup**\
**!find**\
**!search**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |
:---|---|---
**!lookup** | **\<type\>** | **\<ID\>**
**!find** | **\<type\>** | **\<ID\>**
**!search** | **\<type\>** | **\<ID\>**
**!lookup** | **\<type\>** | **\<name\>**
**!find** | **\<type\>** | **\<name\>**
**!search** | **\<type\>** | **\<name\>** 
>Types: item, skill, mob, npc, map (non-case sensitive)\
Prints search result in the user’s chatbox.

\
**!addnx**\
Level: **Tester**

Format: |  |
:---|---
**!addnx** | **\<amount\>**
>Gives the user the specified amount of NX.

\
**!nx**\
**!setnx**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!nx** | **\<amount\>**
**!setnx** | **\<amount\>**
>Sets the user's NX to the specified amount.

\
**!dp**\
**!setdp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!dp** | **\<amount\>**
**!setdp** | **\<amount\>**
>Sets the user’s DP to the specified amount.

\
**!vp**\
**!setvp**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!vp** | **\<amount\>**
**!setvp** | **\<amount\>**
>Sets the user’s VP to the specified amount.

\
**!goto**\
Inherited from Swordie. Level: **Tester**

Format: |
:---|
**!goto** |
>Prints list of valid maps in user’s chatbox.

**!goto \<map\>** |
---|
>Warps user to the specified map.\

\
**!cleardrop**\
**!cleardrops**\
Level: **Tester**

>Remove drops from the field.

\
**!savemap**\
Inherited from Swordie. Level: **Tester**

Format: |
:---|
**!savemap list** |
>Prints list of saved maps in the user’s chatbox.

**!savemap** | **save** | **\<identifier\>**
---|---|---
>Save the user’s current map location using the specified identifier (until the next server restart).

**!savemap** | **go** | **\<identifier\>**
---|---|---
>Warps the user to the specified map.

\
**!warriorequips**\
Inherited from Swordie. Level: **Tester**
>Gives the user a set of warrior equips.

\
**!mageequips**\
Inherited from Swordie. Level: **Tester**
>Gives the user a set of mage equips.

\
**!archerequips**\
Inherited from Swordie. Level: **Tester**
>Gives the user a set of bowmen equips.

\
**!thiefequips**\
Inherited from Swordie. Level: **Tester**
>Gives the user a set of thief equips.

\
**!pirateequips**\
Inherited from Swordie. Level: **Tester**
>Gives the user a set of pirate equips.

\
**!clearinv**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |  |
:---|---|---|---
**!clearinv** | **\<type\>** | **\<start index** | **\<end index\>**
>Types: equip, use, etc, setup, cash (non-case sensitive)\
(Also valid: pet, consume, special, install, eq)\
Clears the user’s inventory in the specified tab, within the specified indices.
    
\
**!nukeinv**\
Level: **Tester**
>Completely clears the user’s inventory.

\
**!mobinfo**\
Inherited from Swordie. Level: **Tester**
>Prints information about the nearest mob.\
(Range of 100 pixels - see **!tag** for information about range)

\
**!completequest**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!completequest** | **\<ID\>**
>Sets the specified quest as completed for the user.

\
**!removequest**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!removequest** | **\<ID\>**
>Sets the specified quest as Not Started, and removes it for the user.

\
**!setguildgp**\
**!guildgp**\
**!setgp**\
Level: **Tester**

Format: |  |
:---|---
**!setguildgp** | **\<amount\>**
**!guildgp** | **\<amount\>**
**!setgp** | **\<amount\>**
>Sets the user's guild GP to the specified amount.

\
**!getguildskill**\
**!guildskill**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!getguildskill** | **\<skill ID\>** | **\<skill level\>**
**!guildskill** | **\<skill ID\>** | **\<skill level\>**
>Gives the user the specified guild skill, with the specified level.

\
**!sethonor**\
**!honor**\
Inherited from Swordie. Level: **Tester**\

Format: |  |
:---|---
**!sethonor** | **\<amount\>**
**!honor** | **\<amount\>**
>Sets the user’s free honour points to the specified amount.

\
**!startquest**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!startquest** | **\<ID\>**
>Sets the specified quest as started for the user.

\
**!bypassskillcd**\
**!ignoreskillcd**\
**!bypasskillcd**\
Inherited from Swordie. Level: **Tester**
>Resets skill cooldowns for the user.

\
**!toggledamagecap**\
Inherited from Swordie. Level: **Tester**
>Self-explanatory.

\
**!shop**\
Inherited from Swordie. Level: **Tester**
>Brings up a universal shop (ID: 1011100)

\
**!mobstat**\
Inherited from Swordie. Level: **Tester**
>Sets the stats of one of the mobs in the user’s map to 1000, with level set to 1, and skillid/itemid/mobskillid set to 145. (Presumably for debug purposes)

\
**!fp**\
**!findportal**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!fp** | **\<ID\>**
**!findportal** | **\<ID\>**
**!fp** | **\<name\>**
**!findportal** | **\<name\>**
>Prints the search results in the user’s chatbox.

\
**!showbuffs**\
Inherited from Swordie. Level: **Tester**
>Prints the user’s currently applied buffs in the user’s chatbox.

\
**!roleplay**\
Level: **Tester**

Format: |  |
:---|---
**!roleplay** | **\<roleplaying character index\>**
>Sets the user’s roleplaying character index to the one specified.

\
**!tohex**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!tohex** | **\<32bit integer\>**
>Converts a decimal (max 2.147b) to hexadecimal and prints the results in the user’s chatbox.

\
**!fromhex**\
Inherited from Swordie. Level: **Tester**

Format: |  |
:---|---
**!tohex** | **\<hex string\>**
>Converts a hexadecimal to decimal and prints the results in the user’s chatbox.

\
**!lookupreactor**\
**!reactors**\
Inherited from Swordie. Level: **Tester**
>Prints the list of reactors in the user’s map.

\
**!script**\
Inherited from Swordie. Level: **Tester**

Format: |  |  |
:---|---|---
**!script** | **\<type\>** | **\<name\>**
>Types: none, npc, field, portal, reactor, item, quest (non-case sensitive)\
Starts the specified script. (Presumably for debug purposes)

\
**!testequips**\
Level: **Tester**
>Gives one piece of equipment of every type.

\
**!reloadbg**\
**!reloadback**\
**!reloadbackground**\
Level: **Tester**
>Re-loads map background.

\
**!disablebg**\
**!removebg**\
Level: **Tester**
>Disable map background.

\
**!objvisible**\
**!obj**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!objvisible** | **\<tag\>** | **\<?\>**
**!obj** | **\<tag\>** | **\<?\>**
>Sets the specified map object as visible - WIP

\
**!objtagvisible**\
**!objtag**\
Level: **Tester**
>No logic implemented - WIP

\
**!gray**\
Level: **Tester**
>Makes the user's background grey.

\
**!actionbar**\
**!ab**\
Level: **Tester**

Format: |  |
:---|---
**!actionbar** | **\<action bar id\>**
>I have no idea what this does. There is scant little documentation about it in the source code.

\
**!ab_usable**\
Level: **Tester**

Format: |  |
:---|---
**!ab_usable** | **\<entry id\>**
>Sets the cooldown for action bar ID 22, with the specified entry ID to 50000ms.\
I have no idea what this does. There is scant little documentation about it in the source code.

\
**!clearozstage**\
Level: **Tester**
>Clear the current Oz stage for the user.

\
**!setobject**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!setobject** | **\<field effect\>** | **\<value\>**
>Sets the specified field effect to the specified value.\
I have no idea what this does. There is scant little documentation about it in the source code.

\
**!setobjectstate**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!setobjectstate** | **\<field object name\>** | **\<mode\>**
>Sets the specified field object to the specified mode.\
I have no idea what this does. There is scant little documentation about it in the source code.

\
**!fps**\
Level: **Tester**
>Starts FPS mode.

\
**!tp**\
**!teleport**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!tp** | **\<x-coordinate\>** | **\<y-coordinate\>**
**!teleport** | **\<x-coordinate\>** | **\<y-coordinate\>**
>Teleports the user to the specified `x` and `y` coordinates.

\
**!hpcraftcount**\
**!hpwashcraftcount**\
**!hpwash**\
Level: **Tester**
>Returns the number of times the user has crafted Red Soul Shards.

\
**!sethpcraftcount**\
**!sethpwashcraftcount**\
**!sethpwash**\
Level: **Tester**

Format: |  |
:---|---
**!sethpcraftcount** | **\<amount\>**
**!sethpwashcraftcount** | **\<amount\>**
**!sethpwash** | **\<amount\>**
>Sets the number of times the user has crafted Red Soul Shards to the specified quantity.

\
**!mpcraftcount**\
**!mpwashcraftcount**\
**!mpwash**\
Level: **Tester**
>Returns the number of times the user has crafted Blue Soul Shards.

\
**!setmpcraftcount**\
**!setmpwashcraftcount**\
**!setmpwash**\
Level: **Tester**

Format: |  |
:---|---
**!setmpcraftcount** | **\<amount\>**
**!setmpwashcraftcount** | **\<amount\>**
**!setmpwash** | **\<amount\>**
>Sets the number of times the user has crafted Blue Soul Shards to the specified quantity.

\
**!randomemotion**\
Level: **Tester**
>The user will start using a random emotion.

\
**!screenmessage**\
Level: **Tester**

Format: |  |
:---|---
**!screenmessage** | **\<message\>**
>Sets the static screen message to the specified message for the user.

\
**!giveandequip**\
Level: **Tester**

Format: |  |  |
:---|---|---
**!giveandequip** | **\<item ID\>** | 
**!giveandequip** | **\<item ID\>** | **\<preserve old\>**
>Gives the user the specified equip item, and wears it for the user.\
`preserve old` defaults to `false` - i.e. the old equipment in the slot will be destroyed.

\
**!setequippedbagindex**\
**!bagindex**\
Level: **Tester**

Format: |  |
:---|---
**!setequippedbagindex** | **help** |
**!bagindex** | **help** |
>Explains the command
 
 Format: |  |  |
:---|---|---
**!setequippedbagindex** | **\<item ID\>** | **\<bag index\>**
**!bagindex** | **\<item ID\>** | **\<bag index\>**
>Searches through all of the users' equip/equipped items, and sets the first item found with the specified ID to the specified (EQUIPPED) bag index.

## Intern level commands:

**!logequipped**\
**!logequippedtoconsole**\
Level: **Intern**
>Log all equipped items to the console & log files.

\
**!logequips**\
**!logequipstoconsole**\
Level: **Intern**
>Log all equip items to the console & log files.

## GameMaster level commands:

**!online**\
Level: **GameMaster**
>Lists players currently online, in the user’s chatbox.

\
**!forceevent**\
Inherited from Swordie. Level: **GameMaster**
>Presumably to force start the next automatic event.

\
**!spawn**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |  |  
:---|---|---
**!spawn** | **\<mob ID\>**
**!spawn** | **\<mob ID\>** | **\<number to spawn\>**
**!spawn** | **\<mob ID\> \<number to spawn\>** | **\<hp of mobs\>**
>Spawns mob(s) with the specified attributes.

\
**!npc**\
**!spawnnpc**\
Level: **GameMaster**

Format: |  |
:---|---
**!npc** | **\<NPC ID\>**
**!spawnnpc** | **\<NPC ID\>** 
>Spawns a temporary NPC (within 50 pixels left/right) of the user.

\
**!tag**\
**!killnear**\
Level: **GameMaster**

Format: |
:---|
**!tag** | 
**!killnear** | 
>Kills players within a 500 pixels range around the user. (see below)

Format: |  |
:---|---
**!tag** | **\<pixels\>**
**!killnear** | **\<pixels\>**
>Kills players in a square the size of the twice the number of pixels provided.

For example if the command **!tag 4** is used the following rectangle is generated: 
```
4 3 2 1 0 1 2 3 4
3               3
2               2
1               1
0       X       0
1               1
2               2
3               3
4 3 2 1 0 1 2 3 4   Where **X** marks the user’s spot, and each number denotes one pixel.
```

\
\
**!warpnear**\
**!warpoutnear**\
Level: **GameMaster**

Format: |  |
:---|---
**!warpnear** | **\<map ID\>**
**!warpoutnear** | **\<map ID\>**
>Warp players within a 500 pixels range around the user to the specified map. (see **!tag** for an example of how the range works)

\
**!healmap**\
**!healall**\
Level: **GameMaster**
>Revive and/or heal HP/MP of all players in the map

\
**!kill**\
Level: **GameMaster**

Format: |  |
:---|---
**!kill** | **\<IGN\>**
>Kills the specified player.

\
**!testreward**\
Level: **GameMaster**

Format: |  |
:---|---
**!testreward** | **\<Item ID\>**
>Sends a packet to get reward results, using the specified item ID. The packet type used by this command isn't used any where else at the moment. (Presumably for debug purposes)   

\
**!pnpc**\
Inherited from Swordie. Level: **GameMaster**

Format: | |
:---|---
**!pnpc** | **\<NPC ID\>**
>Spawns a permanent NPC (within 50 pixels left/right) of the user. (NPC saved into database)

\
**!forcechase**\
Inherited from Swordie. Level: **GameMaster**
>Makes mobs in the user’s map chase the user.

\
**!setcontroller**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |
:---|---
**!setcontroller** | **\<IGN\>**
>Makes mobs in the target’s map chase the target.

\
**!traitexp**\
Level: **GameMaster**

Format: |  |  |
:---|---|---
**!traitexp** | **\<type\>** | **\<amount\>**
>Types: charm, willpower, insight, charisma, sense (non-case sensitive)\
Adds the specified amount of trait exp to the specified trait.

\
**!mobcontroller**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |
:---|---
**!mobcontroller** | **\<IGN\>**
>Prints the mobs chasing the target in the target’s map, in the user’s chatbox. (Presumably for debug purposes)

\
**!proitem**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |  |  |  |
:---|---|---|---|---
**!proitem** | **\<ID\>** | **<\Stats\>** | **\<WA & MA\>** | **\<Flamed Stats\>**
>Gives the user an equipment with the specified stats.\
Stats: STR, DEX, INT, LUK\
Flames: Boss Damage %, IED %, All Stat %

\
**!getitem**\
**!item**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |  |
:---|---|---
**!item** | **\<ID\>**
**!getitem** | **\<ID\>**
**!item** | **\<ID\>** | **\<amount\>**
**!getitem** | **\<ID\>** | **\<amount\>**
**!item** | **\<name\>**
**!getitem** | **\<name\>**
**!item** | **\<name\>** | **\<amount\>**
**!getitem** | **\<name\>** | **\<amount\>**
>Gives the user the specified item.

\
**!mesos**\
**!money**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |
:---|---
**!mesos** | **\<amount\>**
**!money** | **\<amount\>**
>Gives the user the specified amount of mesos.

\
**!ohko**\
**!oko**\
Level: **GameMaster**

>Sets all mobs in the map to 1 HP.

\
**!ld**\
**!liedetector**\
Level: **GameMaster**

Format: |  |
:---|---
**!ld** | **\<IGN\>**
**!liedetector** | **\<IGN\>**
>Sends Lie Detector to the specified player.

Format: |  |
:---|---
**!ld** | **@me**
**!liedetector** | **@me**
>Sends Lie Detector to the user to test LDs.

\
**!ban**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |  |  |  |
:---|---|---|---|---
**!ban** | **\<IGN\>** | **\<amount\>** | **\<type\>** | **\<reason\>**
>Types: min, hour, day, year (non-case sensitive)\
(Also valid: m, mins, h, hours, d, days, y, years )\
Bans the specified user for the specified duration, and records the reason for ban.

\
**!killmobs**\
Inherited from Swordie. Level: **GameMaster**
>Kills all mobs in the user’s map. (Drops disabled)

\
**!givenx**\
Inherited from Swordie. Level: **GameMaster**

Format: |  |  |
:---|---|---
**!givenx** | **\<IGN\>** | **\<amount\>**
>Awards the specified player with the specified amount of NX.

\
**!giveexp**\
Level: **GameMaster**

Format: |  |  |
:---|---|---
**!giveexp** | **\<IGN\>** | **\<amount\>**
>Awards the specified player with the specified amount of EXP.

\
**!giveitemmap**\
Level: **GameMaster**

Format: |  |  |
:---|---|---
**!giveitemmap** | **\<ID\>**
**!giveitemmap** | **\<ID\>** | **\<amount\>**
>Gives every player in the map the specified item (of the specified amount, if applicable).

\
**!warp**\
Level: **GameMaster**

Format: |  |
:---|---
**!warp** | **\<IGN\>**
>Warps the user to the target.

\
**!summon**\
Level: **GameMaster**

Format: |  |
:---|---
**!warp** | **\<IGN\>**
>Warps the target to the user.

\
**!giveeqto**\
Level: **GameMaster**
>Brings up a NPC dialog that allows you to select a piece of equipment to gift, and input a player to gift it to.

\
**!testrewardbox**\
Level: **GameMaster**
>Gives the user rewards (item IDs: 1542063, 1442223) via reward box.

\
**!getrune**\
Level: **GameMaster**
>Returns the X and Y coordinates of the rune in the map.

\
**!spawnrune**\
Level: **GameMaster**
>Spawns a rune in the map.

\
**!spawnrunetype**\
Level: **GameMaster**

Format: |  |
:---|---
**!spawnrunetype** | **\<rune type\>**
>Spawns a rune of the specified type in the map.\
Types: 0 to 8

\
**!openweb**\
Level: **GameMaster**
>Opens up Brandon's GitHub page. (Presumably for debug purposes)

\
**!rotatecam**\
Level: **GameMaster**

Format: |  |  |
:---|---|---
**!rotatecam** | **\<degree\>** | **\<duration\>**
>Rotates the user's screen by the specified degree, for the specified duration.

\
**!hyperstatforlvl**\
Level: **GameMaster**

Format: |  |
:---|---
**!hyperstatforlvl** | **\<level\>**
>Returns to number of hyperstat points the user would have gotten by the specified level.

\
**!userexplode**\
Level: **GameMaster**
>Makes all users in the map explode.

\
**!quiz**\
Level: **GameMaster**
>Sends some quiz-related packet to all players in the field. No idea what this does, since the methods called are only used in this command. Presumably for debug purposes.

\
**!openui**\
Level: **GameMaster**

Format: |  |
:---|---
**!openui** | **\<UI ID\>**
>Opens the UI with the specified ID for the user.

\
**!closeui**\
Level: **GameMaster**

Format: |  |
:---|---
**!closeui** | **\<UI ID\>**
>Closes the UI with the specified ID for the user.

\
**!eventskill**\
Level: **GameMaster**
>Calls (skill) Smokescreen Shell for the user.

\
**!addpendantslot**\
Level: **GameMaster**

Format: |  |
:---|---
**!addpendantslot** | **\<days\>**
>Increases the additional pendant slot duration by the specified number of days.

\
**!admin**\
**!fly**\
**!adminmode**\
Level: **GameMaster**
>Allows the user to use skills in maps where they're disabled.

\
**!whitechat**\
**!white**\
Level: **GameMaster**
>Toggles the user's chat colour (normal vs GM's white chat).  

\
**!itemsmega**\
**!itemmega**\
**!itemega**\
Level: **GameMaster**

Format: |  |  |
:---|---|---
**!itemsmega** | **\<item ID\>** | **\<message\>**
**!itemmega** | **\<item ID\>** | **\<message\>**
**!itemega** | **\<item ID\>** | **\<message\>**
>Sends an Item Megaphone with the specified item and message (and with whisper disabled).

## Admin level commands:

**!test**\
Inherited from Swordie. Level: **Admin**
>Some kind of skill effect shows - presumably to let you know if Admin-level commands can be issued. (Presumably for debug purposes)

\
**!packet**\
Inherited from Swordie. Level: **Admin**

Format: |  |  |
:---|---|---
**!packet** | **\<op\>** | **\<data\>**
>Sends packet with the provided opcode. (Presumably for debug purposes)

\
**!testcts**\
**!cts**\
Inherited from Swordie. Level: **Admin**
>Presumably gives a buff in the form of Kaiser’s Final Trance, that sets a bunch of temporary stats to 0. (Presumably for debug purposes)

\
**!atom**\
Inherited from Swordie. Level: **Admin**
>No idea what this does. Does something to the stats of the mobs in the user’s map.\
Throws NPE due to faulty logic (i.e. calling `get(number of lives in the field - 1)` on a map of object ID to Life).

\
**!sendQRvalue**\
**!qr**\
Level: **Admin**

Format: |  |  |
:---|---|---
**!sendQRvalue** | **\<Quest ID\>** | **\<QR Value\>**
**!qr** | **\<Quest ID\>** | **\<QR Value\>**
>Send a QRValue with the specified quest ID and value.

\
**!clearcache**\
Inherited from Swordie. Level: **Admin**
>Stops active scripts the user has running, and clear server cache (recursive for Worlds).\
Cache includes: Drop, Field, Item, Mob, NPC, Quest, Skill, Reactor.

\
**!reloadcs**\
Inherited from Swordie. Level: **Admin**
>Reloads the Cash Shop (Affects: server-wide)

\
**!maplepoints**\
Level: **Admin**

Format: |  |
:---|---
**!maplepoints** | **\<amount\>**
>Gives the user the specified amount of Maple Points.

\
**!dropinstance**\
**!testinstancedrop**\
**!testinstanceddrop**\
Level: **Admin**

Format: |  |
:---|---
**!dropinstance** | **\<Item ID\>**
**!testinstancedrop** | **\<Item ID\>**
**!testinstanceddrop** | **\<Item ID\>**
>Drops an instanced drop with the specified item ID at the user's location. (For debug purposes)

Format: |  |
:---|---
**!dropinstance** | **preset**
**!testinstancedrop** | **preset**
**!testinstanceddrop** | **preset**
>Drops Chaos Vellum drops at the user's location. (For debug purposes)

\
**!hide**\
Level: **Admin**
>Hides the user.

\
**!commercilevel**\
Level: **Admin**

Format: |  |
:---|---
**!commercilevel** | **\<level\>**
>Sets the Commerci ship level to the specified level.

\
**!commercipacket**\
Level: **Admin**

Format: |  |
:---|---
**!commercipacket** | **\<type\>**
>Supposed to send a commerci voyage packet based on the specified type.\
Does not work at the moment as the packet-writing has been commented out.

\
**!eventrank**\
**!eventrankings**\
Level: **Admin**
>Sends the event rank packet to all users in the map.

\
**!flagracerank**\
Level: **Admin**
>Update ranking for the field.
