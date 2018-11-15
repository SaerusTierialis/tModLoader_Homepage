These idea are not final. If you have feedback or ideas, please share them on our [Discord](https://discord.gg/KXf9zen).


Abilties should do one or more of the following:
* Have a risk/reward element
* Require skill or timing to use
* Create a new playstyle


Abilities should NOT:
* Be "press and forget"
* Grant free damage with no downside


1. Novice
    * No abilities. Low, balanced stats. Power scales all damage types.

1. Melee
    * Base ability could be a toggle to increase damage at the cost of defense or vice versa.

    1. Knight (rename?)
        * Basic damage class
        * no good ideas yet
        
    1. Berserker
        * Attack speed class with a rage mechanic of some kind
        * maybe shouts/warcrys?
        
    1. Guardian
        * Tank class
        * abilities focusing on blocking, generating threat, and perhaps reflecting damage
        * blocking just before recieving an attack should have a bonus

1. Ranged
    * Base ability might be a gravity trap that is enhanced by the subclasses
    
    1. Sniper
        * High damage, crit-focused
        * Snipe ability locks the player in place (even in the air) and prevents the use of weapons/items. The player can then shoot off a few very powerful attacks. The player will be able to end the ability early.
        * Snipe deals bonus damage to enemies caught in the trap
    
    1. Engineer
        * Utility class
        * Can deploy a floating turret that slowly follows the player. The turret consumes a resource will it is out and the resource regenerates while stowed away. The player can scoop up the turret as needed.
        * Decision: turret will either aim towards the cursor or aim at the nearest npc
        * Decision: turret will either attack when the player attacks or on its own
        * Decision: turret projectiles might be fixed or might be based on the weapon equipped when turret was deployed
        * Turret has some interaction with enemies caught in the trap (fire a missle?)
        * Turret might have a support aura and/or debuff aura for added utility
        * Turret will scale with both ranged and minion
        * While the turret is out, player damage is decreased. The overall damage will be slightly increased if both the player and turret are hitting. The idea is that the turret is not just "free damage", but instead allows you to attack from multiple locations/angles.

1. Magic
   * Base ability might be a resource that fills by spending mana and can be expended for a buff that increases damage, but stops mana regen.
    
    1. Elementalist
        * Damage magic class
        * Elemental attunement mini-game. Use the ability to start rotating through 4 elements (fire/water/earth/air). Use the ability again to select the current element. Each element grants a different buff for a duration.
        * Selecting oppsite elements consecutively (fire+water or earth+air) causes the buff to fail, the history to reset, and might consume life/mana.
        * Once you have used all 4 elements at lease once without failing, you will trigger all 4 buffs together for an extended duration.
        * Overall, this class offers primarily damage-focused buffs at the cost of mana and attention.
     
     1. Sage/Seer/Mystic
         * Utility class
         * No good ideas yet

1. Thief
   * Speedy class that can use any weapons except minion
   * Base ability could be stealth, a burst of speed, etc

   1. Assassin
         * Attacks from stealth to deal bonus damage
         * Can use any weapons except minion
   
   1. Ninja
         * Throwing-focused class
         * No good ideas yet
   
   1. Name needed (previously the ranged-only gunslinger)
         * A class that triggers bonus attacks (or spells) by attacking at precise moments
         * Attacking that the right times increases combo and triggers a bonus attack. Attacking at the wrong time breaks combo. Reaching a certain combo count triggers a burst of attacks and resets the combo.
         * The idea is to deal damage through good timing and reacting instead of holding down the attack button as usual. The desired effect is burst damage and minimal resource consumption (bullets/mana/etc). This may be the most skill-based class.

1. Minion
      * Base ability can recall minions to your location. 

      1. Soul Binder
         * Focuses on having a few very strong minions
         * Can sacrafice minion capacity for minion damage. Use the skill repeatedly to cycle through the amount of slots to sacraficed. The overall damage is increased. For example, giving up 1 of 3 minion slots would increase minion damage by >50%.
         * Can toggle on soul binding. This further increases minion damage, but gives each minion a life bar. Minions take damage from projectiles. When the player is hit, the nearest minion also takes damage. When a minion dies, the player takes a decent chunk of damage. Reducing minion cap with the above ability increases minion life. Minion life will regenerate slowly.
         * Will have an ability to heal minions using the player's own life.
         * The two toggle abilities can only be used when no minions are currently summoned
         * These abilities do not affect sentries
      
      1. Minion Master
         * Gains more control over minions
         * An ability to teleport minions to the cursor
         * An toggle ability that keeps minions near the player. This can be used to allow grounded ranged minions to be used in the air (e.g., tiki) or to keep minions together when moving.
         * An ability that actively commands minions... possibly by throwing them at your enemies. This ability would have a per-minion cooldown. Peraps the ability would select the minion nearest the cursor and then throw them in the direction that you move the mouse?
      
      1. Sentry Class (or lack thereof)
         * The way that sentries are implemented is very messy and hard to work with. Most sentries don't even use sentry capacity and instead just have a hard limit of one per sentry type. No sentry class is planned at this time, but I might revisit this once the other classes are complete. I personally enjoy sentries so I would eventually like to find a way to make it work.
      
1. Support
      * Mostly unchanged. See [here](./Temporary_Rework_User_Documentation.md)
      * Will have a toggle ability that converts damage bonuses of any weapon type into healing power to allow flexible itemization. This ability cannot be used with the hybrid ability that makes equipment affect all damage types.

1. Hybrid (tier 2) and Hybrid Prime (tier 3)
      * Scales all damage types equally
      * Toggle ability to allow damage bonuses from equipment to apply to all damage types (perhaps at 80% value?)
      * Has a resource bar for each damage type except minion
      * Using a weapon while you have its resource offers a large damage boost
      * Using a weapon while its resource is depleted incurs a large damage penalty
      * Every time that you use a weapon, its resource will deplete for a few seconds (not based on attack speed or damage dealt)
      * When any 2 of the 4 resources are emptied, all 4 resources refill
      * The desired effect is that players are rewarded for using multiple damage types (any combination of melee/ranged/magic/thowing) and penalized for using just one
      * Some ideas for enhancing this through passives:
         * When 1 resource is emptied, the other damage types gain a larger bonus
         * Bonus defense while wielding a melee weapon when the melee resource is not empty
         * Bonus mana regen when the magic resource is empty (replenish mana after you've used magic to empty the resource)
      * Note re minions:
         * Most minion weapons use a snapshot of the minion damage so including it here would be very overpowered (minions would keep the bonus after the resource is emptied)
         * The class will still scale minion damage so you can use minions fairly well alongside the other damage types
