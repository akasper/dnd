# Stats
How to convert current characters to the test system.

### Health
A number of health levels indicating how much damage you have taken.

> The number of health you have is based on your size.
>
> Fine:         1
> Diminutive:   2
> Tiny:         3
> Small:        4
> Medium:       5
> Large:        6
> Huge:         7
> Gargantuan:   8
> Collosal:     9


### Resistance
Your damage threshold for taking one box of damage.

> Calculate your Resistance like this:
> [health] + [CON+] + [clvl] + [warmor] + [narmor] + [hp]/10 (round down)

* _CON+_: Your Constitution bonus
* _health_: The number of health boxes you have when unwounded
* _clvl_: Your character level. Do not include template levels
* _warmor_: The armor bonus from your worn armor
* _narmor_: Your natural armor bonus
* _hp_: Your current hitpoints


#### Healing Magic
Healing magic behaves differently.

> Cure ___ Wounds spells heal varying levels of health.
> Light:      1 health level
> Moderate:   2 health levels
> Serious:    3 health levels
> Critical:   4 health levels
> Heal:       5 health levels
>

Mass versions of these spells scale accordingly.


#### Fast Healing, Regeneration
Still not sure what to do with these.

#### Temporary Hit Points
Temporary Hit Points increase your resistance until you take at least one level
of damage from a single attack. After you have taken the damage, your resistance
is immediately lowered back to its normal level.

> Example:
> Noriam has a Resistance of 12. He is granted 3 temporary hit points from a
> spell, giving him a resistance of 15 until he takes at least one level of
> damage (or the spell expires).
>
> In combat, Noriam is hit by an attack dealing 27 points of damage. Because
> this is enough to exceed his resistance threshold for one level of damage,
> but not enough to exceed it for two levels of damage (30), Noriam takes a
> single level of damage and his resistance returns to 12.


#### Damage Resistance, elemental resistance
Damage resistance and elemental resistance behave per the normal rules for
calculating them.


### Prowess
Your combat aptitude.

> Your Prowess is equal to your base attack bonus.

Prowess is based on your _base_ attack bonus, not your _calculated_ attack
bonus. Only base attack bonus increases earned by adding class levels count
towards your prowess. Attack bonus increases for high attributes, weapon focus,
or other bonuses do not count.

#### Stance
Every combat round, on your turn, you divide your prowess between attack and
defense. This allocation is known as your stance.


#### Attack Bonus

> Calculate your melee attack rolls as follows:
> [d20] + [att] + [STR+] + [size] + [mods]

* _d20_: The natural value on the roll of a d20. See "weapons" for more details
* _att_: Your current attack stance
* _STR+_: Your Strength bonus
* _size_: Your size modifier (according to table 8-1, p134 of the PHB)
* _mods_: Miscellaneous modifiers for feats, situational modifiers, magical
bonuses, etc.

> Calculate your ranted attack rolls as follows:
> [d20] + [att] + [DEX+] + [size] + [range] + [mods]

* _d20_: The natural value on the roll of a d20. See "weapons" for more details
* _att_: Your current attack stance
* _DEX+_: Your Dexterity bonus
* _size_: Your size modifier (according to table 8-1, p134 of the PHB)
* _range_: The range penalty, based on your distance to the target.
* _mods_: Miscellaneous modifiers for feats, situational modifiers, magical
bonuses, etc.

#### Defense
Replaces Touch AC.

> Calculate your Defense as follows:
> 10 + [def] + [DEX+] + [size] + [mods]

* _def_: Your current defense stance
* _DEX+_: Your Dexterity bonus
* _size_: Your size modifier (according to table 8-1, p134 of the PHB)
* _mods_: Miscellaneous modifiers for feats, situational modifiers, magical
bonuses, etc.
