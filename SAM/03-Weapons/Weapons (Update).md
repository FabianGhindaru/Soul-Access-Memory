
## 1. Choosing Your Weapon

Every Protagonist carries **one Melee and one Ranged weapon** at all times. Switching between them is Free.

- **Melee** weapons roll **d6s**, scale with **Body**, have **higher base dice** (2d6), and use Melee Range.
- **Ranged** weapons roll **d8s**, scale with **Mind**, start at **1d8**, and default to Medium Range.

Pick one family from each category below. The family determines your weapon's **special trait**.

---

## 2. Melee Weapon Families

All Melee families use **2d6 (CF 5)** base, scaling with Body. 
**Default Range:** Melee.

### Blunt
_Hammers, clubs, batons, fists with weight behind them._
**Overpower:** Push the target up to 3 tiles in any direction on hit.

### Slash
_Swords, knives, claws, anything with an edge._
**Deadly Precision:** Apply 🩸Drain on Crit.

### Pierce
_Spears, rapiers, needles, focused stabbing weapons._
**Collateral Damage:** Deal half the damage dealt (rounded down) as Entropy damage to all Enemies adjacent to the target.

### Thrown
_Javelins, throwing axes, darts, shuriken, boomerangs._
**Tribe Instinct:** Cadence. Throw the weapon at a Being. Returns at the end of your current turn. Range is dictated by your Throwing power.

### Lash
_Whips, chains, flexible weapons._
**Unbounded:** Short Range instead of Melee.

### Brawl
_Gauntlets, brass knuckles, martial arts, improvised strikes._
**One-two Combo:** CF is doubled (CF 10 instead of CF 5).

---

## 3. Ranged Weapon Families

All Ranged families use **1d8 (CF 3)** base, scaling with Mind. 
**Default Range:** Medium.

### Pistol
_Handguns, sidearms, compact firearms._
**Quick Draw:** Drawing this weapon from Inventory allows a Free attack with it.

### SMG
_Submachine guns, burst-fire weapons._
**Spray & Pray:** Gain one additional damage die (effectively +1 tier; e.g. 1d8 → 2d8 at T1–4). Any die that rolls a 1 removes the CF from the Attack Sequence once. SMG base CF is 7 instead of 3.

### Rifle
_Semi-automatic rifles, battle rifles, combat carbines._
**Steady Shot:** Crits add +15 Lethality instead of +10.

### Sniper
_High-caliber precision rifles, anti-materiel weapons._
**Fathomless:** Long Range instead of Medium.

### Heavy
_Miniguns, grenade launchers, heavy ordnance._
**Explosive Power:** Targets all Enemies in Short Range of the target. Can only be fired **once per turn (Attack Cadence)**.

### Exotic
_Unique, atypical, or custom-built weapons._
**Depends on the specific weapon.**

---

## 4. Weapon Quality

All weapons fall into one of three quality tiers. Higher quality adds a flat bonus to your Attack Value and grants more upgrade slots.

| Quality | Weapon Bonus | Upgrade Slots | Description |
| ------- | :----------: | :-----------: | ----------- |
| **Basic** | +0 | 1 | Standard-issue, scrap-built, or unmodified |
| **Refined** | +5 | 2 | Quality craftsmanship, tuned, or lightly modded |
| **Masterpiece** | +10 | 3 | Pinnacle weaponry, custom-forged, legendary |

### Upgrade Slots
Upgrades can be equipped on weapons at any time, but using them requires the specific skills. Unless stated otherwise, Upgrades can be changed from one weapon to another freely.

---

## 5. How Damage Works

### The Attack Value Formula
When you attack, your **Attack Value (AV)** is:
```
AV = Dice Rolls + Weapon Bonus (+ CF when Chaining)
```

| Part                     | What It Is                                                                                                          |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| **Dice Rolls**           | Your weapon's dice, scaled by your Attribute tier (see below)                                                       |
| **Weapon Bonus**         | +0, +5, or +10 based on weapon quality                                                                              |
| **CF (Chaining Factor)** | A fixed value used only as the follow-up when **Chaining** two attacks together. CF is pre-written on every weapon. |

The defender compares their **Defense Value (Mitigate or Dodge)** against your AV:
```
DV = Dice Rolls + Armor Values (+ CF when Chaining)
```

### Dice Scaling With Your Attribute
As your Attribute grows, your weapon dice increase. This happens automatically at the same breakpoints as your Check Dice Pool.

| Attribute Tier | Melee (Body) | Ranged (Mind) |
| -------------- | ------------ | ------------- |
| **1–4**        | 2d6 (CF 5)   | 1d8 (CF 3)    |
| **5–8**        | 3d6 (CF 5)   | 2d8 (CF 3)    |
| **9–12**       | 4d6 (CF 5)   | 3d8 (CF 3)    |

CF remains fixed regardless of tier unless specified otherwise.

### Chaining Factor (CF)
CF is used as the follow-up value when **Chaining** two attacks into one. When you Chain, your primary attack rolls normally, then you add the follow-up weapon's CF to the AV. 



---

## 6. Crits (Explode System)

A Crit triggers when **any die in your attack roll shows its natural maximum** (e.g., a 6 on a d6, an 8 on a d8). All Crit dice **Explode**: roll an extra die of the same type and add it to the total. If that die also shows its maximum, it explodes again.

When **multiple dice crit** in the same attack, add only **one extra die** total.

### Melee Crits (d6)
- Trigger: Natural **6**.
- Effect: Explode (add 1d6). Repeat on successive 6s.
- No flat bonus. **More consistent** — 16.7% chance per die (up to 4 dice).

### Ranged Crits (d8)
- Trigger: Natural **8**.
- Effect: Explode (add 1d8) **AND** add a flat **+10 Lethality Bonus** to the AV.
- Repeat on successive 8s. **More devastating** — 12.5% chance per die (up to 3 dice).

---

## 7. Quick Reference

### Melee Families at a Glance

| Family | Base | CF | Key Trait |
| ------ | ---- | --- | ------------------------------------------------ |
| Blunt | 2d6 | 5 | Push target up to 3 tiles on hit |
| Slash | 2d6 | 5 | Crits apply 🩸Drain |
| Pierce | 2d6 | 5 | Half damage as Entropy to adjacent enemies |
| Thrown | 2d6 | 5 | Cadence. Throw weapon, returns end of turn |
| Lash | 2d6 | 5 | Short Range instead of Melee |
| Brawl | 2d6 | **10** | CF doubled |

### Ranged Families at a Glance

| Family | Base | CF | Key Trait |
| ------ | ---- | --- | ------------------------------------------- |
| Pistol | 1d8 | 3 | Draw allows for a Free attack |
| SMG | 1d8* | 7 | Spray & Pray (+1 die); 1s remove CF once |
| Rifle | 1d8 | 3 | +5 AV if you didn't move this turn |
| Sniper | 1d8 | 3 | Crits: +15 Lethality instead of +10 |
| Heavy | 1d8 | 3 | Once per turn; AoE in Short Range |
| Exotic | Varies | Varies | Defined per weapon |

*\*SMG effectively rolls 1 additional die via Spray & Pray; CF 7 reflects 2d8 base.*

### Expected AV by Tier & Quality (Standard Families)

| Tier | Melee Dice | CF | Basic | Refined (+5) | Masterpiece (+10) |
|------|-----------|-----|-------|-------------|-------------------|
| 1–4 | 2d6 (8.4) | 5 | **13.4** | **18.4** | **23.4** |
| 5–8 | 3d6 (12.6) | 5 | **17.6** | **22.6** | **27.6** |
| 9–12 | 4d6 (16.8) | 5 | **21.8** | **26.8** | **31.8** |

| Tier | Ranged Dice | CF | Basic | Refined (+5) | Masterpiece (+10) |
|------|------------|-----|-------|-------------|-------------------|
| 1–4 | 1d8 (6.6) | 3 | **9.6** | **14.6** | **19.6** |
| 5–8 | 2d8 (13.1) | 3 | **16.1** | **21.1** | **26.1** |
| 9–12 | 3d8 (19.7) | 3 | **22.7** | **27.7** | **32.7** |

*\*Dice parenthetical is expected value including crits. This table is for reference only.*
