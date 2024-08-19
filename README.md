**This project aims to update and maintain the MikScrollingBattleText (MSBT) addon, which may have been abandoned, while the original author continues their updates or if the project remains unmaintained.**

# MikScrollingBattleText (MSBT)

MSBT is designed to be an extremely lightweight, efficient, and highly configurable mod that makes it easier to see combat information by scrolling the information on the screen in separate, dynamically creatable scroll areas. It is a replacement for Blizzard's Floating Combat Text and Damage output.

## Features

- Lightweight and efficient design.
- Scroll incoming damage/heals, outgoing damage/heals, and notifications in separate configurable scroll areas on the playing field.
- Display player and pet cooldown completion alerts.
- Display loot alerts with a total of how many are now in inventory.
- Add triggers that will allow you to show notifications based on a variety of conditions.
- Assign a sound file to play for events/triggers.
- Dynamically create new scroll areas and assign any event/trigger to them.
- Customize the position, size, animation style, enabled state, font style, font size, font outline, and opacity for each of the scroll areas.
- Customize each individual event's color, font style, font size, font outline, opacity, output message, enabled state, and scroll area.
- Set "Master Font" settings that will be inherited by all of the scroll areas and the events in them unless they are overridden at the scroll area or event level.
- Merge AoE data into one event with cumulative damage/healing done with number of normal and crits specified.
- Show overhealing amounts against yourself or party/raid members.
- Color unit names according to their class.
- Color damage amounts according to damage type.
- Show partial effects (resists, absorbs, vulnerabilities, etc) colored according to type.
- Filter output information with a full suite of spam controls.
- Load on demand options.
- For mod developers:
    - Output your own scrolling messages with the MikSBT.DisplayMessage function instead of having to create your own frame and animation code. You can also use your own font by first registering it with MSBT via the MikSBT.RegisterFont function.
    - Create custom animation styles.
    - See the included API.html file for reference information.

## Supported Events

- Incoming:
    - Melee Damage, Misses, Dodges, Parries, Blocks, Deflects, Absorbs, and Immunes.
    - Skill Damage, Damage Over Time (DoTs), Misses, Dodges, Parries, Blocks, Deflects, Absorbs, Immunes, Reflects, and Interrupts.
    - Spell Resists.
    - Heals and Heals Over Time (HoTs).
    - Pet Melee Damage, Misses, Dodges, Parries, Blocks, Deflects, Absorbs, and Immunes.
    - Pet Skill Damage, Damage Over Time (DoTs), Misses, Dodges, Parries, Blocks, Deflects, Absorbs, and Immunes.
    - Pet Spell Resists.
    - Pet Heals and Heals Over Time (HoTs).
    - Environmental Damage.
- Outgoing:
    - Melee Damage, Misses, Dodges, Parries, Blocks, Deflects, Absorbs, Immunes, and Evades.
    - Skill Damage, Damage Over Time (DoTs), Misses, Dodges, Parries, Blocks, Deflects, Absorbs, Immunes, Reflects, Interrupts, and Evades.
    - Spell Resists and Buff Dispels.
    - Heals and Heals Over Time (HoTs).
    - Pet Melee Damage, Misses, Dodges, Parries, Blocks, Deflects, Absorbs, Immunes, and Evades.
    - Pet Skill Damage, Damage Over Time (DoTs), Misses, Dodges, Parries, Blocks, Deflects, Absorbs, Immunes, and Evades.
    - Pet Spell Resists and Buff Dispels.
    - Pet Heals and Heals Over Time (HoTs).
- Notification:
    - Buffs / Buff Stacks / Buff Fades.
    - Debuffs / Debuff Stacks / Debuff Fades.
    - Item Buffs / Item Buff Fades.
    - Enter/Leave Combat.
    - Power Gains and Losses.
    - Alternate Power Gains and Losses.
    - Chi Gains and Chi Full.
    - Combo Point Gains and Combo Points Full.
    - Holy Power Changes and Holy Power Full.
    - Honor Gains.
    - Reputation Gains and Losses.
    - Skill Gains.
    - Experience Gains.
    - Killing Blows (Player and NPC).
    - Extra Attacks.
    - Soul Shard Creation.
    - Enemy Buff Gains.
    - Monster Emotes.
    - Player, Pet, and Item Cooldown Completions.
- Loot:
    - Looted Items.
    - Money Gains.
- Default Triggers:
    - All Relevant Classes - Low Health, Low Mana, Low Pet Health.
    - Death Knight - Killing Machine, Rime, Shadow Infusion x5.
    - Druid - Berserk, Clearcasting, Predator's Swiftness, Shooting Stars.
    - Hunter - Kill Shot, Lock and Load.
    - Mage - Brain Freeze, Clearcasting, Fingers of Frost, Missile Barrage.
    - Monk- Elusive Brew x5, x10, x15, Mana Tea x20, Vital Mists x5.
    - Paladin - Hammer of Wrath, The Art of War.
    - Priest - Clearcasting, Shadow Orb x3.
    - Rogue - Blindside.
    - Shaman - Clearcasting, Lava Surge, Maelstrom Weapon x5, Tidal Waves.
    - Warlock - Decimation, Molten Core, Nightfall.
    - Warrior - Bloodsurge, Execute, Revenge, Sudden Death, Taste for Blood, Victory Rush.

## Commands

```sh
/msbt	        Shows the options interface.
/msbt reset	    Resets the current profile to the default settings.
/msbt disable	Disables the mod.
/msbt enable	Enables the mod.
/msbt version   Shows the current version.
/msbt help	    Shows the command usage.
```

## Installation

1. Download ziped addon from [release page](https://github.com/Placidina/MikScrollingBattleText/releases).
2. Extract the files and place the folder in `World of Warcraft/_retail_/Interface/AddOns/`.
3. Enable the addon from the character selection screen in World of Warcraft.

For more details, visit the [official CurseForge page](https://www.curseforge.com/wow/addons/mik-scrolling-battle-text).