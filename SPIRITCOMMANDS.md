Full list of commands available to GMs
Date of Creation: 19/8/2020
Date last Updated: 19/8/2020
Maintained by: KOOKIIE

Note on account types and their level of access:
0x00000000 : Player
0x00000020 : Tester
0x00000008 : Intern
0x00000010 : GameMaster
0x00000010 : Admin


Player level commands:

!map
Inherited from SwordieMS. Level: Player
Prints a System Notice of all characters in the user’s map


Tester level commands:

!showinvinfo or !invinfo
Inherited from SwordieMS. Level: Tester
Prints out the name, generic item ID, specific item ID, bag index, and inventory type, for every item in inventory, in the user’s chatbox. (Presumably for debug purposes)

!checkid or !getid or !charid
Inherited from SwordieMS. Level: Tester
Prints out the user’s character ID and account ID, in the user’s chatbox. (Presumably for debug purposes)

!getphantomstolenskills
Inherited from SwordieMS. Level: Tester
Prints out skills the user has stolen as a Phantom, in the user’s chatbox. (Presumably for debug purposes)

!stealskilllist
Inherited from SwordieMS. Level: Tester
Steals every skill. (Presumably for debug purposes)

!np or !nearestportal
Inherited from SwordieMS. Level: Tester
Prints out map and portal information (within 30 pixels) for the map the user is in, in the user’s chatbox. (Presumably for debug purposes)

!stats
    Inherited from SwordieMS. Level: Tester
Prints out the user’s stats, in the user’s chatbox. (Presumably for debug purposes)

!testdrop
    Inherited from SwordieMS. Level: Tester
Format:
!testdrop <mob ID>
!testdrop <mob ID> <amount>
Spawns the specified mob (with 3 HP). (Presumably for debug purposes)

!done
Inherited from SwordieMS. Level: Tester
Sets level to 235, HP/MP to 250,000, stats to 1000

!hypertp
    Inherited from SwordieMS. Level: Tester
    Gives the user a Hyper Teleport Rock

!job or !setjob
Inherited from SwordieMS. Level: Tester
Format:
!job <ID> or !setjob <ID>
Set the user’s job to the job ID specified.

!sp or !setsp
Inherited from SwordieMS. Level: Tester
Format:
!sp <amount> or !setsp <amount>
Give the user the specified amount of free SP in the user’s highest level skill tab.

!ap or !setap
Inherited from SwordieMS. Level: Tester
Format:
!ap <amount> or !setap <amount>
Give the user the specified amount of free AP.

!hp or !sethp
Inherited from SwordieMS. Level: Tester
Format:
!hp <amount> or !sethp <amount>
Set the user’s Max HP to the specified amount.

!mp or !setmp
Inherited from SwordieMS. Level: Tester
Format:
!mp <amount> or !setmp <amount>
Set the user’s Max HP to the specified amount.

!str or !setstr
Inherited from SwordieMS. Level: Tester
Format:
!str <amount> or !setstr <amount>
Set the user’s STR to the specified amount.

!dex or !setdex
Inherited from SwordieMS. Level: Tester
Format:
!dex <amount> or !setdex <amount>
Set the user’s DEX to the specified amount.

!int or !setint
Inherited from SwordieMS. Level: Tester
Format:
!int <amount> or !setint <amount>
Set the user’s INT to the specified amount.

!luk or !setluk
Inherited from SwordieMS. Level: Tester
Format:
!luk <amount> or !setluk <amount>
Set the user’s LUK to the specified amount.

!level or !setlevel or !lvl or !lv
Inherited from SwordieMS. Level: Tester
Format:
!level <amount> or !setlevel <amount> or !lvl <amount> or !lv <amount>
Set the user’s Level to the specified amount. (Stats not changed)
!leveluntil or !levelupuntil
Inherited from SwordieMS. Level: Tester
Format:
!leveluntil <amount> or !levelupuntil <amount>
Recursively level the user up till to the specified amount. (Stats not changed)

!heal
Inherited from SwordieMS. Level: Tester
Format:
!heal <amount>
Recovers the user’s HP and MP by the specified amount. (capped at Max HP/MP)

!curhp
Inherited from SwordieMS. Level: Tester
Format:
!curhp <amount>
Sets the user’s current HP to the specified amount.
!curmp
Inherited from SwordieMS. Level: Tester
Format:
!curmp <amount>
Sets the user’s current MP to the specified amount.

!invincible
Inherited from SwordieMS. Level: Tester
Toggles the user’s invincibility.

!morph
Inherited from SwordieMS. Level: Tester
Format:
!morph <ID>
Not entirely sure what this does, tbh. It sets the option value to the specified morph ID, and the option’s skill ID to Kaiser’s Final Trance, before pushing the buff via the TSM.

!mount
Inherited from SwordieMS. Level: Tester
Format:
!mount <ID>
See above (sets the option value to the specified mount ID), but it also sets the user to be riding.
!testtempstat
Inherited from SwordieMS. Level: Tester
No idea what this does. Does something to the stats of the mobs in the user’s map.

!setmap
Inherited from SwordieMS. Level: Tester
Format:
!setmap <map ID>
Warps the user to the specified map.

!setportal
Inherited from SwordieMS. Level: Tester
Format:
!setportal <portal ID>
Warps the user to the specified portal

!getskill
Inherited from SwordieMS. Level: Tester
Format:
!getskill <skill ID> <current level> <max level>
Gives the user the specified skill with the specified current and max levels.

!maxskills
Inherited from SwordieMS. Level: Tester
Max skills for non-Evan classes.
(Buggy tester command using janky/hacky logic)

!lookup or !find or !search
Inherited from SwordieMS. Level: Tester
Format:
!lookup <type> <ID> or !find <type> <ID> or !search <type> <ID>
!lookup <type> <name> or !find <type> <name> or !search <type> <name> 
Types: item, skill, mob, npc, map (non-case sensitive)
Prints search result in the user’s chatbox.

!nx or !setnx
Inherited from SwordieMS. Level: Tester
Format:
!nx <amount> or !setnx <amount>
Gives the user the specified amount of NX.
!dp or !setdp
Inherited from SwordieMS. Level: Tester
Format:
!dp <amount> or !setdp <amount>
Sets the user’s DP to the specified amount.

!vp or !setvp
Inherited from SwordieMS. Level: Tester
Format:
!vp <amount> or !setvp <amount>
Sets the user’s VP to the specified amount.

!goto
Inherited from SwordieMS. Level: Tester
Format:
!goto
Prints list of valid maps in user’s chatbox.
!goto <map>
Warps user to the specified map.
Note to devs: Consider making the hashmap a constant, since a new hashmap is generated every time a user calls this command.

!savemap
Inherited from SwordieMS. Level: Tester
Format:
!savemap list
Prints list of saved maps in the user’s chatbox.
!savemap save <identifier>
Save the user’s current map location using the specified identifier.
!savemap go <identifier>
Warps the user to the specified map.

!warriorequips
Inherited from SwordieMS. Level: Tester
Gives the user a set of warrior equips.

!mageequips
Inherited from SwordieMS. Level: Tester
Gives the user a set of mage equips.
!archerequips
Inherited from SwordieMS. Level: Tester
Gives the user a set of bowmen equips.

!thiefequips
Inherited from SwordieMS. Level: Tester
Gives the user a set of thief equips.

!pirateequips
Inherited from SwordieMS. Level: Tester
Gives the user a set of pirate equips.

!clearinv
Inherited from SwordieMS. Level: Tester
Format:
!clearinv <type> <start index> <end index>
    Types: equip, use, etc, setup, cash (non-case sensitive)
        (Also valid: pet, consume, special, install, eq)
Clears the user’s inventory in the specified tab, within the specified indices.
    
!nukeinv
    Level: Tester
    Completely clears the user’s inventory.
    (Not guaranteed to work.)

!mobinfo
Inherited from SwordieMS. Level: Tester
Prints information about the nearest mob.
(Range of 100 pixels - see !tag for information about range)

!completequest
Inherited from SwordieMS. Level: Tester
Format:
!completequest <ID>
Sets the specified quest as completed for the user.

!removequest
Inherited from SwordieMS. Level: Tester
Format:
!removequest <ID>
Sets the specified quest as Not Started, and removes it for the user.
!sethonor or !honor
Inherited from SwordieMS. Level: Tester
Format:
!sethonor <amount> or !honor <amount>
Sets the user’s free honour points to the specified amount.

!startquest
Inherited from SwordieMS. Level: Tester
Format:
!startquest <ID>
Sets the specified quest as started for the user.

!bypassskillcd or !ignoreskillcd or !bypasskillcd
Inherited from SwordieMS. Level: Tester
Resets skill cooldowns for the user.

!toggledamagecap
Inherited from SwordieMS. Level: Tester
Self-explanatory.

!shop
Inherited from SwordieMS. Level: Tester
Brings up a universal shop (ID: 1011100)

!mobstat
Inherited from SwordieMS. Level: Tester
Sets the stats of the mobs in the user’s map to 1000. (Presumably for debug purposes)

!fp or !findportal
Inherited from SwordieMS. Level: Tester
Format:
!fp <ID> or !findportal <ID>
!fp <name> or !findportal <name>
Prints the search results in the user’s chatbox.

!showbuffs
Inherited from SwordieMS. Level: Tester
Prints the user’s currently applied buffs in the user’s chatbox.
!tohex
Inherited from SwordieMS. Level: Tester
Format:
!tohex <32bit integer (2.1b)>
Converts a decimal to hexadecimal and prints the results in the user’s chatbox.

!fromhex
Inherited from SwordieMS. Level: Tester
Format:
!tohex <hex string>
Converts a hexadecimal to decimal and prints the results in the user’s chatbox.

!lookupreactor or !reactors
Inherited from SwordieMS. Level: Tester
Prints the list of reactors in the user’s map.

!script
Inherited from SwordieMS. Level: Tester
Format:
!script <type> <name>
Types: none, npc, field, portal, reactor, item, quest (non-case sensitive)
Starts the specified script. (Presumably for debug purposes)


Intern level commands:



GameMaster level commands:

!online
Level: GameMaster
Lists players currently online, in the user’s chatbox.

!forceevent
Inherited from SwordieMS. Level: GameMaster
Presumably to force start the next automatic event.
!spawn
Inherited from SwordieMS. Level: GameMaster
Format:
    !spawn <mob ID>
!spawn <mob ID> <number to spawn>
!spawn <mob ID> <number to spawn> <hp of mobs>
Spawns mob(s) with the specified attributes.

!npc or !spawnnpc
Level: GameMaster
Format:
    !npc <NPC ID> or !spawnnpc <NPC ID> 
Spawns a temporary NPC (within 50 pixels left/right) of the user.

!tag or !killnear
Level: GameMaster
Format:
    !tag or !killnear
Kills players within a 500 pixels range around the user. (see below)
    !tag <pixels> or !killnear <pixels>
Kills players in a square the size of the twice the number of pixels provided.
E.g. !tag 4
4 3 2 1 0 1 2 3 4
3        3
2        2
1        1
0            X    0
1        1
2        2
3        3
4 3 2 1 0 1 2 3 4 Where X marks the user’s spot.

!warpnear or !warpoutnear
Level: GameMaster
Format:
    !warpnear <map ID> or !warpoutnear <map ID> 
Warp players within a 500 pixels range around the user to the specified map. (see !tag for an example of how the range works)

!healmap or !healall
Level: GameMaster
Revive and/or heal HP/MP of all players in the map
!kill
Level: GameMaster
Format:
    !kill <IGN>
Kills the specified player.

!pnpc
Inherited from SwordieMS. Level: GameMaster
Format:
    !pnpc <NPC ID>
Spawns a permanent NPC (within 50 pixels left/right) of the user. (NPC saved into database)

!forcechase
Inherited from SwordieMS. Level: GameMaster
Makes mobs in the user’s map chase the user.

!setcontroller
Inherited from SwordieMS. Level: GameMaster
Format:
!setcontroller <IGN>
Makes mobs in the target’s map chase the target.

!traitexp
    Level: GameMaster
Format:
!traitexp <type> <amount>
Types: charm, willpower, insight, charisma, sense (non-case sensitive)
Adds the specified amount of trait exp to the specified trait.

!mobcontroller
    Inherited from SwordieMS. Level: GameMaster
Format:
!mobcontroller <IGN>
Prints the mobs chasing the target in the target’s map, in the user’s chatbox. (Presumably for debug purposes)
!proitem
Inherited from SwordieMS. Level: GameMaster
Format:
!proitem <ID> <Stats> <WA & MA> <Flamed Stats>
Gives the user an equipment with the specified stats.
Stats: STR, DEX, INT, LUK
Flames: Boss Damage %, IED %, All Stat %

!getitem or !item
Inherited from SwordieMS. Level: GameMaster
Format:
!item <ID> or !getitem <ID>
!item <ID> <amount> or !getitem <ID> <amount>
!item <name> or !getitem <name>
!item <name> <amount> or !getitem <name> <amount>
Gives the user the specified item.

!mesos or !money
Inherited from SwordieMS. Level: GameMaster
Format:
!mesos <amount> or !money <amount>
Gives the user the specified amount of mesos.

!ld or !liedetector
Inherited from SwordieMS. Level: GameMaster
Format:
!ld <IGN> or !liedetector <IGN>
Sends Lie Detector to the specified player.
!ld @me or !liedetector @me
Test the command.

!ban
Inherited from SwordieMS. Level: GameMaster
Format:
!ban <IGN> <amount> <type> <reason>
Types: min, hour, day, year (non-case sensitive)
(Also valid: m, mins, h, hours, d, days, y, years )
Bans the specified user for the specified duration, and records the reason for ban.

!killmobs
Inherited from SwordieMS. Level: GameMaster
Kills all mobs in the user’s map. (Drops disabled)
!givenx
Inherited from SwordieMS. Level: GameMaster
Format:
!givenx <IGN> <amount>
Awards the specified player with the specified amount of NX.

!giveitemmap
    Level: GameMaster
Format:
!giveitemmap <ID>
!giveitemmap <ID> <amount>
Gives every player in the map the specified item (of the specified amount, if applicable).

!warp
    Level: GameMaster
Format:
!warp <IGN>
Warps the user to the target.

!summon
    Level: GameMaster
Format:
!warp <IGN>
Warps the target to the user.

!giveeqto
    Level: GameMaster
Brings up a NPC dialog that allows you to select an equipment to gift, and input a player to gift it to.


Admin level commands:

!test
Inherited from SwordieMS. Level: Admin
Some kind of skill effect shows - presumably to let you know if Admin-level commands can be issued. (Presumably for debug purposes)

!packet
Inherited from SwordieMS. Level: Admin
Format: !packet <op> <data>
Sends packet with the provided opcode. (Presumably for debug purposes)
!testcts or !cts
Inherited from SwordieMS. Level: Admin
Presumably gives a buff in the form of Kaiser’s Final Trance, that sets a bunch of temporary stats to 0. (Presumably for debug purposes)


!atom
Inherited from SwordieMS. Level: Admin
No idea what this does. Does something to the stats of the mobs in the user’s map.

!clearcache
Inherited from SwordieMS. Level: Admin
Stops active scripts the user has running, and clear server cache (recursive for Worlds).
Cache includes: Drop, Field, Item, Mob, NPC, Quest, Skill, Reactor.

!reloadcs
Inherited from SwordieMS. Level: Admin
Reloads the Cash Shop (Affects: server-wide)

!maplepoints
Level: Admin
Format:
!maplepoints <amount>
Gives the user the specified amount of Maple Points.
