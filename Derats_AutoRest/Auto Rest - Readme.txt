This module was created at the request of DrAzTIK, who wanted to be able to recover his spells between battles, as in Dragon Age Origin (or Pillars of Eternity).

The module has two components:
1: Automatic rest :
Selectable: How to apply rest:
- By pressing a key (D, non-configurable). This simulates a rest in the game
- Automatically after each battle. This simulates the behavior of recent games such as Pillars of Eternity or Dragon Age Origine.
- Both. Because there isn't always a battle to trigger the end-of-battle script.

Your choice: Which rest?
- All spells restored + 3D8 hp restored
- All spells restored + 3D8 hp restored + Dispel 100%
- All spells restored + Heal
- All spells restored + Heal + Dispel 100%
- All spells restored + Restoration
- All spells restored + Restoration + Dispel 100%
- All spells restored + Resurrection + Restoration
- All spells restored + Resurrection + Restoration + Dispel 100%

2: Players can't die (requires the first component)
Your choice: How to avoid death?
- Minimum hit points set at 1 (players can still die by spells/effects of death/petrification/disintegration)
- Minimum hit points set at 1 + simulated death (when players are down to 1 or 2 hp, they become unusable and are replaced by a tombstone) (which lasts until the end of the battle or pressing the D key, depending on what has been chosen for the first component)
- Minimum hit points set at 1 + Immunity to all forms of death (but pjs can still die from a characteristic set to 0 (Illithids))
- Minimum hit points set at 1 + simulated death + Immunity to all forms of death

Warning: Simulated Death has one drawback: "dead" players replaced by a tombstone no longer run scripts and therefore don't respond to the D key. So if ALL players are "dead", you can't exit this mode, and you have to reload.
You can consider that if ALL players are "dead", it's game-over.



Notes:
- Pressing the D key doesn't work if the AI is deactivated. Automatic rest after battles is always active.
- Heal simulates the legal "rest until healed" option.
- 100% dissipation simulates the dissipation of buffs after rest.
- the standard rest simulation is "3D8 hp rendered or Heal, + dissipation, by pressing D". All other combinations are cheating. (Then again, pressing the D key doesn't bother to check if enemies are present or if the area doesn't allow rest).
- If you want to change the key needed to activate rest, simply edit the "drazres2.baf" file (before installing) and change the line "HotKey(D)" to "HotKey(the key you want)".



Version history :
version 0.5:Beta: first version, Rest + automatic Heal after each fight.
version 1: 	added "Rest + Major restoration".
version 2: 	Added "Rest + Major restoration + resurrection".
			Added "press D" management.
version 3: 	Added the possibility of Dissipation.
version 4: 	Correction of "press D" management.
			Removal of a choice step at installation.
			Added healing limited to 3D8.
			Added read_me.
Version 5: 	Added English translation.
Version 6: 	Added "Players can't die" option with its subcomponents.
			Removed "no log" in TP2 (which could accumulate appends in scripts).
			Added English readme.
			Added routine for installing mod on OBG2/BGT.
			Options for the main component and the second component now require the main component.
Version 6.1: The OBG2 routine is useless.
			Missing sring error corrected (typo error).