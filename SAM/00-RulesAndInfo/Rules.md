***


# SAM RULESET - Revised Edition

## Table of Contents
1.  **Core Mechanics & Attributes**
2.  **Resolution & Checks**
3.  **Combat Structure (The Rhythm)**
4.  **Movement & Range**
5.  **Attack & Defense (The Clash)**
6.  **Special Combat Mechanics (Burn, Chain, Targeting)**
7.  **Status Effects & Procs**
8.  **Fading, Death & Restoration**
9.  **Manifestations & Augments**
10. **Ability Style Guide**
11. **Mnemonic Skills & Advancement**
12. **Environmental Rules (Downpour)**
13. **Reference Tables**

---

## 1. Core Mechanics & Attributes

### Protagonist Definition
Every Protagonist (player character) is defined by three fundamental Attributes: **Body**, **Mind**, and **Soul**. These Attributes form the foundation of your character and influence everything from combat prowess to social interactions.

*   **Attribute Range:** 0 to 12.
*   **Protagonist Level:** Calculated as `(Body + Mind + Soul) ÷ 3`, rounded down.
*   **Attribute Modifier:** Calculated as `Attribute Score ÷ 2`, rounded up. (e.g., Attribute 9 = 4.5 → 5 Modifier).

### Body
Body represents physical capabilities—strength, speed, endurance, and awareness of the physical world.
*   **In Combat:** Determines Max Health, Movement, Mitigation Defense, and Melee Attack Bonus.
*   **Out of Combat:** Feats of strength, enduring hardship, physical senses, and close-quarters intimidation.

### Mind
Mind embodies mental acuity—intelligence, intuition, charisma, and reflexes.
*   **In Combat:** Determines Turn Order, Dodge Defense, and Ranged Attack Bonus.
*   **Out of Combat:** Solving puzzles, reading people, persuasion, and reacting to changes.

### Soul
Soul reflects connection to the intangible—creativity, luck, empathy, and mnemonic powers.
*   **In Combat:** Determines Healing Threshold, Known Manifestations, Known Augments, and Arcane Attack Bonus.
*   **Out of Combat:** Creative problem-solving, benefiting from fortune, emotional connection, and supernatural perception.

---

## 2. Resolution & Checks

### The Dice Pool
When attempting an action where the outcome is uncertain, the Conductor calls for an **Attribute Check**. Your ability to succeed is determined by your Attribute Score.

| Attribute Points | Dice Pool | Rating |
| :--- | :--- | :--- |
| 0 - 4 | 1d6 | Beginner |
| 5 - 8 | 2d6 | Adept |
| 9 - 12 | 3d6 | Expert |

### Reading the Bones (Success & Explosions)
Roll your dice pool and read each die individually to count your Hits.
*   **1 - 3:** Failure (0 Hits).
*   **4 - 5:** Success (1 Hit).
*   **6:** Critical (1 Hit + Explode).
    *   **The Explode Rule:** If you roll a 6, count it as a Hit, then reroll only that die. If the new roll is 4-5-6, gain another Hit. Continue rerolling only as long as you roll 6s.

*   **Note:** You do not add Attribute Modifiers to dice pools unless a skill explicitly states otherwise.
*   **Critical Success:** Rolling maximum value on all dice (e.g., all 6s on 3d6 before exploding) grants a DEVIL.

### Difficulty Ratings
The Conductor sets the Difficulty based on task complexity. Difficulty equals the number of Hits required to succeed.
*   **1 (Standard):** Hacking a basic terminal, sensing a lie.
*   **2 (Hard):** Picking a master lock, persuading a hostile guard.
*   **3 (Heroic):** Hacking a mainframe while under fire.

### Versus Checks (Contested Actions)
When competing directly (e.g., grapple, lie to inquisitor), both roll.
1.  **Compare Hits:** Most Hits wins.
2.  **Tiebreaker:** Higher Attribute Modifier wins. If using a Derived Check, use the highest Attribute Modifier between the two Attributes involved.

### Derived Checks
Complex actions require two Attributes in unison. Roll the dice pool of your **lowest** Attribute among the two.
*   **Grit (Body + Mind):** Physical control + mental focus. (e.g., Stealth, surgery).
*   **Aura (Body + Soul):** Physical expression + spiritual emotion. (e.g., Dancing, animal handling).
*   **Will (Mind + Soul):** Logical acuity + intuitive connection. (e.g., Deception, insight).

### Attribute Mastery Skills
Gain skills to mitigate bad luck. **Restriction:** Declare after rolling; only one Mastery Skill per Check.

| Level | Skill | Effect |
| :--- | :--- | :--- |
| 2 | Intention | Exhaust. Reroll any number of 1s. |
| 6 | Precision | Exhaust. Replace one die with your Attribute Modifier (1-6). If 6, it explodes. |
| 10 | Prowess | Once per session. Turn one die into a natural 6 (guaranteed Hit + explode). |

---

## 3. Combat Structure (The Rhythm)

### Initiative & Rounds
Combat is divided into Rounds. Each Round, all participants act once in Initiative Order.

#### Start of Combat
Sort all player characters (PCs) by descending Mind attribute score. PCs act in this order automatically—no discussion or rolling required.
*   **Turn Order:** PCs with higher Mind scores act first.
*   **Enemy Order:** Enemies always act after all PCs, regardless of their Mind score (e.g., PC with Mind 1 acts before enemy with Mind 4).
*   **PC Ties:** If two PCs have the same Mind score, they choose the order among themselves. This decision can be made at the start of combat or changed each round when out of danger.
*   **Bosses and Minibosses:** Can act in PC order if specified by the Conductor before combat begins. The Conductor decides where in the PC order the Boss acts.

#### The Round Flow
1.  **Start of Turn:** Refresh your 2 Full Beats (4 Half-Beats) and defenses (Mitigate/Dodge 1/round).
2.  **Surprise (Round 1 Only):** Ambushed side acts last. Surprised beings cannot use Swift or Cadence abilities.
    *   If PCs are ambushed: Order inverts (Enemies first, then PCs).
    *   If Enemies are ambushed: Order remains standard (PCs first, then Enemies), but enemies lose Swift/Cadence.
3.  **End of Round:** Trigger status effect (SE) damage/procs, then remove all unproc'd SEs.

### Action Economy (Beats)
Combat is measured in Beats. Think of these as your "time currency" for the round.

#### Your Turn Allowance
*   **Start of Turn:** You gain 2 Full Beats (equals 4 Half-Beats).
*   **End of Turn:** Any unused Beats are lost.

#### Action Types
| Action Type | Cost | Description |
| :--- | :--- | :--- |
| **Major Action** | 2 HB (1 FB) | Attack (Melee/Ranged), Cast a Manifestation, or use a complex skill. |
| **Minor Action** | 1 HB | Interact with an item, throw an object, swap weapons, or use an item. |
| **Free Action** | 0 Beats | Open doors, pass through a window, speak one short sentence (~6-8 words). Used for cinematic quick actions. |

#### Movement (Free & Fluid)
Movement does not cost Beats. During your turn, you have a **Movement Pool**.
*   **Base Pool:** 6 tiles.
*   **Attribute Bonus:** Max Movement = 6 + Body Attribute (e.g., Body 7 = 13 tiles).
*   **Weaving:** You can spend tiles from your pool at any point during your turn, splitting it between actions.
*   **No Dash:** Your Max Movement pool is your limit per turn.
*   **No Difficult Terrain:** Tiles are an obfuscation. You may define 1 tile = 1 meter, but this is up to the Conductor.

### Weapon Loadout & Inventory
*   **Primary Weapons (Always Equipped):** 1 Melee Weapon and 1 Ranged Weapon. These are always ready. Switching between them is Free (0 Beats).
*   **Inventory (6 Slots):** Additional weapons, tools, or items.
*   **Declaring Primaries:** Declare Primary Melee and Ranged when out of danger.
*   **No Restrictions:** You can hold a massive Greatsword and a Heavy Sniper Rifle simultaneously. No "handedness" penalties.
*   **No Ammo:** Ammo is infinite. Reloading is Free.
*   **Drawing:** Drawing an item from inventory costs 1 Half-Beat (Minor Action). Once drawn, it is active until swapped again.

---

## 4. Movement & Range

### Range Zones
All Ranges include adjacent tiles plus everything up to their respective distance away.
*   **Melee:** Adjacent tiles only.
*   **Short Range:** Up to 3 tiles.
*   **Medium Range:** Up to 6 tiles.
*   **Long Range:** Up to 9 tiles.
*   **Very Long Range:** Up to 12 tiles.

### Grid
*   **Hex Grids:** 6 adjacent tiles.
*   **Square Grids:** 8 adjacent tiles (orthogonal and diagonals).
*   **Adjacent Definition:** Any tile sharing an edge.

### Fall Damage
Falling deals 5 Melee damage per 3 tiles (Short Range) fallen after the first 3. Essentially, you only start taking fall damage if you fall more than Medium Range (6 tiles or more).
*   5 tiles fall = 0 damage.
*   6 tiles fall = 5 damage.
*   9 tiles fall = 10 damage.
*   Counts as an AV against you (can be Mitigated or Dodged).

---

## 5. Attack & Defense (The Clash)

### The Attack Sequence
**Step 1: The Attack**
The Attacker rolls: `[Dice + Modifiers + Bonuses] = Attack Value (AV)`

**Step 2: The Defense**
The Defender chooses one of three options:
| Option | Cost | Mechanic |
| :--- | :--- | :--- |
| **Take It** | Free | Take full damage (no prevention). |
| **Mitigate** | 1/round | Use Damage Reduction. Subtract your Mitigation Defense Value (MDV) from the incoming damage. `Incoming - MDV`. |
| **Dodge** | 1/round | Use All or Nothing. Compare your Dodge Defense Value (DDV) vs the AV. If DDV is Higher, take 0 damage. If DDV is Lower, take full damage. |

*   **Note:** Defense Values follow the same formula as attacks (Roll + Modifier + Bonus). Limit: Players can use Mitigate once and Dodge once per round. Enemies use tokens.

**Step 3: Resolve Damage**
If AV results in ≥1 damage after defenses, apply to HP. Status effects, procs, or special abilities trigger only on ≥1 damage.

### Damage Calculation (Order of Operations)
When calculating final damage, apply modifiers in this strict order:
1.  **Base AV:** Roll + Modifiers + Bonuses.
2.  **Weakness (Attacker Side):** If defender is Weak to this damage type: `AV × 2`.
3.  **Defense Value (DV):** Defender rolls/calculates their DV.
4.  **Resistance (Defender Side):** If defender is Resistant to this damage type: `DV × 2`.
5.  **Status Effect Penalties:** Apply to DV (e.g., Twist: `DV - 5`).
6.  **Compare AV vs DV:** Resolve defense choice.
7.  **Final Damage:** Calculate damage after defense.

### Damage Types
*   **Default:** Melee, Ranged, Arcane all deal standard damage.
*   **Entropy:** Special SE/Proc damage. Cannot be Mitigated or Dodged. Weak/Resistant/Immune work normally.
*   **Aeon:** Unstoppable "true damage." Ignores all defenses, resistance, immunity, and damage reduction. You simply take the damage as rolled.

### Crits
**Trigger:** A Crit occurs when any die in your Attack Roll shows its Natural Maximum (e.g., 4 on d4, 6 on d6, 12 on d12).

**Resolution:**
1.  **Crit Trigger:** Trigger any ability with a crit condition (e.g., Crits applies Drain).
2.  **Precision Damage:**
    *   **Single-Die Weapons (Precision):** Double the value of the dice roll to the final AV. (e.g., 1d12 crit -> 24). Note: this only doubles the roll, not the whole AV.
    *   **Multi-Die Weapons (Saturation):** Add the Chaining Factor (CF) to the damage once (e.g., 3d6 CF 8 -> +8 AV).

---

## 6. Special Combat Mechanics

### Targeting Rules
*   **Core Rule:** You may only target a specific enemy with one Attack Sequence per turn (unless using a Chain). You may use available Beats to attack *different* enemies in separate sequences.
*   **Attack Sequence Definition:** A single Major Attack, a declared Chain, or a Multi-target attack (AoE).
*   **Why this rule exists:** Prevents a single player from easily stripping an enemy's defenses alone. Multiple PCs must coordinate.

### Defensive Burn (Emergency Defense)
If you have used your defenses for the round but are attacked again, you may push yourself.
*   **Cost:** Gain 1 Burn Token.
*   **Effect:** Immediately perform a Mitigate OR Dodge against the current attack.
*   **Recovery:** At the start of your next turn, each Burn Token reduces your available Beats by 1 Full-Beat.
*   **Token Removal:** Remove all Burn Tokens at the end of your turn.
*   **Max Burn:** You may only Burn twice per turn. Next turn begins with 0 Beats if maxed.
*   **Restriction:** No Offensive Burn. You cannot Burn to gain additional attacks.

### Chaining (Combo Attacks)
Combine two attacks into a single Attack Value against one enemy.

**How it Works:**
1.  **Declare Chain:** Select a Primary Attack (Standard Roll) and a Follow-up Attack (Fixed Value).
2.  **Calculate Cost:** Sum of both attacks (usually 2 HB + 2 HB = 4 HB Total).
3.  **Range Rule:** Range of both attacks must match (Melee/Melee or Ranged/Ranged). Exception: Ranged + Melee is valid if Ranged is Point Blank.
4.  **Calculating CF (Chaining Factor):** All dice/weapons have a pre-written CF. `Total Maximum Dice Value / 2 - 1`.
    *   1d12 = 5 CF; 1d8 = 3 CF; 1d4 = 1 CF; 3d6 = 8 CF.

**The Resolution:**
Roll once with a bonus.
`Primary Roll (AV) + Follow-up CF = Final AV`.
*   **Example:** Sword (1d8 roll 14, CF 3) + Dagger (CF 1). Spend 4 HB. Final AV = 14 + 1 = 15.

**Chain Interactions:**
*   **Manifestation Chain:** You can imbue spells (e.g., Firestarter) onto weapons (e.g., SMG) to add CF and effects (like Burst).
*   **Multi-Damage Types:** Combining Arcane + Melee creates an attack that is both. Weakness/Resistance interact fully. If a target is Weak to Arcane (x2) and Resistant to Melee (DV x2), modifiers cancel out.
*   **AoE Exception:** If a Chain includes an AoE, the entire Chain is spent on that AoE sequence. The second attack's CF is added to damage, but it does not create a separate attack sequence.

---

## 7. Status Effects & Procs

Status Effects (SE) deal Entropic Damage and have unique triggers called PROCs. SEs stack once per type. Applying a 2nd stack procs and removes it.

### General Rules
1.  **Removal:** All SEs are removed automatically at the end of the afflicted Being's turn (unless PROC'd earlier).
2.  **PROC Trigger:** If you apply an SE to a target already affected by that SE, the PROC happens instantly, and that SE is removed.
3.  **Damage:** SE damage is Entropy type (cannot be Mitigated/Dodged, but Weak/Resistant/Immune apply).

### The Effects

#### 1. BURST (Physical: Fire, Ice, Explosion)
*   **Standard Effect:** Target takes 5 Entropy damage at the end of their turn.
*   **PROC (Explosion):** All beings in Short Range take 5 Entropy damage. The target takes 10 Entropy damage.
*   **Result:** Burst removed immediately.

#### 2. DRAIN (Spiritual: Bleed, Poison, Siphon)
*   **Standard Effect:** Target takes 5 Entropy damage if they perform an Offensive Action OR spend Movement. If they do neither, Drain is removed without damage.
*   **PROC:**
    *   **Backlash:** Target takes 10 Entropy damage.
    *   **Siphon:** Attacker heals 5 HP (Overflowing).
*   **Result:** Drain removed immediately.

#### 3. TWIST (Mental: Dizziness, Confusion)
*   **Standard Effect:** Target suffers -5 to all Defense Values (MDV/DDV) for the duration (active until end of turn).
*   **PROC:**
    *   **Impair:** Target's next Attack Value is reduced by -10.
    *   **Adrenaline:** Attacker gains +5 Movement immediately.
*   **Result:** Twist removed immediately.

---

## 8. Fading, Death & Restoration

### Max HP
`10 + 1d4 per Body Attribute` (Max 12d4). Min 10, Max 58, Avg 34.

### Fading Mechanics
Triggered when HP ≤ 0.
*   **Action Economy:** You have 1 Full Beat (2 Half-Beats). You cannot Chain attacks.
*   **Movement:** 3 tiles maximum per turn.
*   **Defenses:** Mitigate (1/round) and Dodge (1/round) unchanged.
*   **Bleed Out:** At the end of your turn, take 5 Entropic Damage.
*   **Exit Fading:** Restore HP > 0.

### Final Threshold (One-Shot Protection)
*   **Rule:** If a single attack (after defenses) would drop your HP to -Max HP or lower, set HP to `-(Max HP - 1)` instead.
*   **Single Attack Definition:** One Attack Value (including Chained), one AoE instance, or one proc effect.
*   **Multiple Attacks:** Damage from separate sources on the same turn count as separate attacks. Protection refreshes when healed above 0.

### Ally Stabilization
An adjacent ally may use a Minor Action (1 HB), once per round per target.
*   **Effect:** Negates Bleed Out until the Fading ally is hit again. Multiple allies can stack stabilization.

### Death Threshold
Permanent Death occurs when HP ≤ -Max HP. No resurrection without specific campaign rules.

### Healing & Keywords
**Healing Threshold (H.T.):**
*   **Rule:** Represents the maximum healing you can receive per round from all sources combined.
*   **Base:** 3 + Mind Attribute. (e.g., Mind 6 = H.T. 9).
*   **Multiple Sources:** Added together and capped at H.T.
*   **Overflow:** Keyword that bypasses H.T.
*   **Out-of-Combat:** After combat ends, automatically heal back to Max HP.

**Keywords:**
*   **Resistant:** DV is doubled.
*   **Immune:** AV is nullified (0 damage).
*   **Weak:** AV against you is doubled.
*   **Combative:** Usable only in combat.
*   **Utility:** Usable only outside combat.
*   **Exhaust:** Usable once per encounter.
*   **Harmless:** Deals no damage.
*   **Swift:** Reactive, can be used outside your turn.
*   **Cadence:** Usable only once per turn.

---

## 9. Manifestations & Augments

Manifestations are rated by Tiers (I–VI). Only 1 Augment can be applied per Manifestation.

### The Casting Sequence
1.  **Declare:** Choose Known Manifestation and Target.
2.  **Form (Optional):** Apply one Augment (Solid, Liquid, Gas, Plasma).
3.  **Amplify (Optional):** Spend additional Beats to Resonate (increase power).
4.  **Create AV:** Same as physical attacks.

### Costs & Scaling
*   **Base Cost:** equals Tier number (e.g., Tier III = 3 HB).
*   **Min Cost:** 2 HB (reduced via Skills).
*   **Resonance:** For every additional Half-Beat spent, Amplify by One Step.
    *   **Effect:** Add +1 Die to the Damage Roll.
*   **Forced Resonance:** Amplifying beyond your Skill Level (or without skill) deals Aeon Damage to self equal to the Max Value of every die added.

### Harmonic Resonance Skill
*   **Effect:** Amplify a number of times equal to your skill level safely.
*   **Requirement:** Soul 2+.
*   **Cost:** 2 MP per level.

### Augments (The Physics)
*   **Default (Pure Energy):** Free. Projectile/Touch. Medium Range.
*   **Crystallize (Solid):** +1 HB. Creates tangible object or physical projectile.
*   **Liquify (Fluid):** +1 HB. Creates hazard puddle.
*   **Vaporize (Gas):** +1 Full Beat. Creates cloud/mist zone.
*   **Ionize (Plasma):** +1 Full Beat. Volatile, conductive energy.

---

## 10. Ability Style Guide

### Structure & Syntax

All abilities, manifestations, and skills must follow this strict structure:

1. Line 1: [Name] (Beat Cost e.g., 1HB) (Beat Cost Icon)
2. (Range) (Damage & Damage Type) (Additional Tags) — Include only if applicable; omit for non-damaging or non-ranged abilities.
3. The Effect Text (A single paragraph of sentences).
4. Flavor/Lore line (optional, in quotes).

#### Beat Cost Icons

- ○ = Free (0 Beats)
- ◐ = Half-Beat (1 HB)
- ● = Full Beat (2 HB)
- ●● = 2 Full Beats (4 HB)

#### Writing Rules

- **Imperative Rule**: Start every sentence with a Concrete Verb (e.g., "Attack...", "Grant...", "Teleport...", "Manifest...", "Push...", "Spend..."). Never use "You" or second-person language.
- **Sentence-Only Rule**: Write the effect as a single paragraph of sentences. No lists, bullet points, or subheadings within the effect text.
- **No Headers**: Define Range, Damage, Keywords, and other mechanics at the beginning of the ability sentence.
- **Defined Terms**: Use consistent terminology like "Being", "Ally", "Enemy", "Short Range", "Medium Range", etc.
- **Tone**: Tactical, Minimal, Confident. Keep descriptions concise and focused on mechanics.
- **Attack Clarity**: All abilities that list a damage line (e.g., 1d4 (CF 1) Arcane) are attacks. The effect text only describes what happens when the attack lands (≥1 damage after defenses). Do not write “Attack a Being” unless the ability performs extra or repeated attacks. Abilities without a damage line are never attacks — simply perform the described effect.
- **One-Verb Rule**: Always start the effect paragraph with a strong imperative verb (e.g., Manifest…, Push…, Spend…, Grant…, Create…, Teleport…).
- **Free Attack Wording**: Only write “Perform a free Attack” or "Expend to attack a Being" when granting a brand-new roll (e.g., summons, tokens, or persistent effects).
- **Defeat/Kill Wording**: Use “defeats the target” instead of “reduces the target to 0 HP or less”.
- **Repeatable/Chain Wording**: For abilities that can fire multiple times in one cast, end with “Repeatable up to X times.” For chains or additions, specify “add +X CF” or similar.
- **Consistency Wins**: Always say “a Being” or “an Enemy”, never “the target” or “it”. Put tags at the start (e.g., Harmless. Combative.) as sentence fragments.
- **Manifestation-Specific**: Manifestation attacks only create their extra effects (barriers, marks, movement, etc.) if the attack deals at least 1 damage after defenses (see Attack Sequence p. 11). For manifestations, range is often fixed and can be omitted if implied.

#### Templates

- **Simple Attack**: Attack a Being.
- **Buff**: Grant an Ally [Benefit] for [Duration].
- **AoE**: Deal [Amount] [Type] damage to all Beings in [Range].
- **Manifestation Example** (range omitted if fixed): Firestarter (Tier I) 1HB ◐ (1d4 (CF 1) Arcane) Manifest a spark that applies 🔥Burst. “Its warmth is part of human nature.”
- **Skill Example**: Lend Expertise FREE(○) (Short Range) Exhaust. Grant an ally your highest Attribute Modifier for their next Attack Value. “Knowledge is made to be shared.”




---

## 11. Mnemonic Skills & Advancement

### Mnemonic Points (MP)
Currency for unlocking skills/epiphanies via narrative trauma or repetition.
*   **Milestone:** Gain 1 MP when increasing an Attribute.
*   **Mission:** Gain 3 MP upon completing a Mission/Gig.

### Acquisition (Dual Path)
1.  **Imprinting (Pay):** Spend listed MP to instantly learn.
2.  **Realization (Play):** Complete the Unlock Condition during gameplay. Skill becomes free immediately.

### Skill List
*   **Apotheosis:** Reduce a specific Manifestation's cost by 1 HB permanently (can be bought multiple times).
*   **Harmonic Resonance:** Safe Amplification of Manifestations.

### Weapon Upgrades
Main way to increase Melee/Ranged damage (besides Attributes).
*   0-3 Upgrade Slots per weapon.
*   Melee upgrades require Body attribute.
*   Ranged upgrades require Mind attribute.

---

## 12. Environmental Rules (Downpour)

While raining, the Conductor rolls the table once at the start of the mission. Effect applies to all combats.
*   **Duration:** Entire mission.
*   **Knowledge:** Players know of Downpour before committing.

| d12 Roll | Effect |
| :--- | :--- |
| 1 | 1 Beat maximum per turn. |
| 2 | Cannot Chain attacks. |
| 3 | Max Movement halved. |
| 4 | Start each combat with Drain. |
| 5 | All Attack Values halved (round down). |
| 6 | All Defense Values halved (round down). |
| 7 | All CF values halved (round down). |
| 8 | Mitigation unavailable (includes Burn). |
| 9 | Dodge unavailable (includes Burn). |
| 10 | One weapon (choose) has 0 CF. |
| 11 | No Attribute Modifiers on Attack Values. |
| 12 | All Attack/Defense Values suffer -5 (min final value 1). |

---

## 13. Reference Tables

### Action Costs Summary
| Action Cost | Type                                 |
| :---------- | :----------------------------------- |
| 2 HB (1 FB) | Major Action (Attack, Manifestation) |
| 1 HB        | Minor Action (Use Item, Draw Weapon) |
| 0 Beats     | Free Action (Open Door, Speak)       |
| Free        | Movement (up to Max Movement pool)   |
| Sum of both | Chain Attack                         |

### Defense Summary
| Defense Type | Cost | Effect |
| :--- | :--- | :--- |
| Take It | Free | Take full damage. |
| Mitigate | 1 use/round | Reduce damage by MDV. |
| Dodge | 1 use/round | All-or-nothing avoidance. |
| Burn (Emergency) | +1 Burn Token | Extra defense, lose HB next turn. |

### Status Effects Summary
| Status Effect | Standard Effect | PROC Effect |
| :--- | :--- | :--- |
| **Burst** | 5 Entropy damage at end of turn. | Explosion (5 dmg to all in Short Range) + 5 dmg to target. |
| **Drain** | 5 Entropy damage if attack/move. | 10 damage + attacker heals 5 (Overflow). |
| **Twist** | -5 to all DV (until end of turn). | Target's next AV -10, attacker +5 Movement. |

### Range Reference
| Range Type | Distance |
| :--- | :--- |
| Melee | Adjacent tiles only. |
| Short | Up to 3 tiles. |
| Medium | Up to 6 tiles. |
| Long | Up to 9 tiles. |
| Very Long | Up to 12 tiles. |

---
