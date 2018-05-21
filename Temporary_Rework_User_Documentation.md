## General Notes
* Classes will have anywhere from 1 to 4 active abilities (most will have 2)
	* Relative to other classes, Cleric/Saint has more abilities and these abilities have more depth
* Abilities are listed in order of unlock
* Unlock is automatic when requirements are met
* Ability mana costs are reduced by mana cost reductions
* Healing does not affect players that have pvp enabled unless you also have pvp enabled and are on their team
* When you gain a duplicate "Status"
	* The longer duration is kept
	* The larger effect magnitude is kept

## New Stats
* **Healing Power**
	* Boosts all healing output from abilities

## Ability Types
* **Passive**
	* Have a constant effect that does not directly pertain to an ability
* **Active**
	* Activated with a hotkey
	* Have mana cost and Cooldown
* **Upgrade**
	* Modify an active Ability
* **Alternate**
	* Adds a second sub-ability to an active ability
	* Sub-ability shares a cooldown with the main active
	* Hold the "Alternate Effect" hotkey when activating the main ability to use the alternate ability instead

## Class Abilities
### Cleric/Saint
* **Passive: Purity (Cleric 10)**
	* Gain 10% Healing Power per debuff immunity up to 100%
	* Supports most vanilla debuffs:
		* Bleeding, Poisoned, OnFire, Venom, Darkness, Blackout, Silenced, Cursed, Confused, Slow, Slimed, OgreSpit, Weak, BrokenArmor, WitheredArmor, WitheredWeapon, CursedInferno, Ichor, Chilled, Frozen, Webbed, Stoned, VortexDebuff, Obstructed, Electrified, Rabies, Burning, Frostburn, Oiled, ShadowFlame, BetsysCurse, Dazed
			* Please let me know if I’ve missed any
* **Active: Heal (Cleric 10)**
	* Mana Cost: 35% of current max mana
	* Cooldown: 3 seconds
	* Large area heal centered on cursor position
	* Activates instantly (i.e., does not require a projectile to “hit”)
	* Requires lines of sight to the cursor and from the cursor to the targets
	* The friendly target nearest the mouse is healed for the full amount while other targets are healed for half
	* Self-healing is reduced
	* A non-pvp player cannot heal a pvp-enabled player
	* Base Value: 20 + ( (level/10) ^ 1.7)
		* Self-heal: 15 + ( (level/10) ^ 1.4)
* **Passive: Cleanse (Cleric 12)**
	* Being afflicted with a debuff (see above list) grants you immunity to the debuff for 120 seconds beginning 10 seconds after the infliction
	* This immunity counts towards the Healing Power stat, cure, and purify
* **Upgrade: Heal - Smite (Cleric 14)**
	* Adds damage to heal
	* The hostile target nearest the mouse is damaged for the full amount while other targets are damaged for half
	* Base Value: 15 + ( (level/10) ^ 2)
		* Scales with Healing Power
	* Deals double damage to NPCs with any of the following in their name:
		* "skel", "zomb", "groom", "bride", "undead", "viking", "eyezor", "bone", "ghost", "ghast", "dark caster", "skull", "dungeon guardian", "mummy", "tim", "ghoul", "diabolist", "floaty gross", "necromancer", "ragged caster", "wraith", "rune wizard", "vampire miner", "frankenstein", "reaper", “undead”, “headless”
			* Please let me know if I’ve missed any
* **Active: Sanctuary (Cleric 16)**
	* Mana Cost: 90% of max mana
	* Cooldown: 120 seconds (can be used on cooldown if NOT replacing)
	* Creates a sanctuary at current location (maximum 1)
	* Sanctuary heals friendly npc and players that have not been hit in the last 10 seconds
	* The healing effect is equal to the full amount of the healing ability once per second
		* No penalty for self-healing
	* If multiple sanctuaries overlap:
		* All non-healing effects will apply, the highest Blessing heal value will be used
		* Only one heal will trigger (which one depends on positioning and order of use; semi-random)
		* There may be some flickering in the blessing visual and inconsistencies in heal timing
	* When leaving a world, sanctuary locations are saved. If the next world that the character enters is the same (based on name) then the sanctuaries will automatically be recreated
	* This is meant to be used for utility and to heal out of combat
	* You do not need to reuse the ability to update healing values or upgrades
* **Update: Sanctuary - Holy Light (Cleric 18)**
	* Affected players also receive a light-generating buff that lasts 120 seconds
* **Alternate: Heal - Barrier (Cleric 20)**
	* Mana Cost: 70% of max mana
	* Creates a wall that knocks back enemies at the cursor location
	* Deals damage equal to a smite
		* Includes bonus damage to undead
	* Lasts for 3 hits or 20 seconds
* **Upgrade: Sanctuary - Blessing (Cleric 23)**
	* Sanctuary now also grants a buff that triggers a heal the next time that the player takes damage within 120 seconds
	* Heal is equal to the heal ability
* **Active: Divine Intervention (Saint 25)**
	* Mana Cost: 50% of max mana
	* Cooldown: 20 seconds
	* Grants nearby allies invincibility for 1.5 seconds
	* Radius is half that of heal
	* Duration is increased 50% on targets wearing Cross Necklace or Star Veil
		* If the Saint is wearing either item, the duration increase applies to everyone
* **Upgrade: Heal - Cure (Saint 30)**
	* Heal now cures other players of any debuffs (see above list) that the saint has immunity to
* **Upgrade: Sanctuary - Link (Saint 35)**
	* Maximum number of sanctuaries increased to 2
	* Hold “Alternate Effect” key to place/replace secondary sanctuary
	* Any player may press “Alternate Effect” key to move between the two sanctuaries so long as they have not been hit in the last 10 seconds
* **Upgrade: Divine Intervention - Radius (Saint 45)**
	* Doubles radius (same as heal)
* **Upgrade: Cure - Purify (Saint 60)**
	* Heal now grants other players 120 second immunity to any debuffs (see above list) that the saint has immunity to
* **Active: Paragon (Saint 70)**
	* Mana Cost: 50% of max mana
	* Cooldown: 300 seconds
	* Cooldown is reduced by valid healing (i.e., does not count overhealing)
		* Each heal reduces Paragon cooldown by 3 seconds if any targets receive valid healing
		* The reduction is tripled for Renew’s full heal
	* Grants a self buff that lasts for 10 seconds
	* Cuts the cooldown and cost of heal in half
	* Instantly refreshes heal’s cooldown
* **Upgrade: Divine Intervention - Duration (Saint 80)**
	* Doubles duration (3 seconds)
* **Alternate: Paragon - Renew (Saint 90)**
	* Mana Cost: 50% of max mana
	* Grants a self buff that lasts for 10 seconds
	* The next valid heal during the buff consumes the buff to heal the closest target to the cursor to full health
		* Does not trigger if the base heal amount is already enough to heal that target to full life (i.e., could trigger on a subsequent heal)
	* Instantly refreshes heal’s cooldown
	* If the buff ends without being used, half of the cooldown is refunded
