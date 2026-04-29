# SAM RULESET – Player Reference

This sheet contains everything you need to play. Omitted from the full rules are Conductor-side procedures, scenario-building notes, and character generation beyond attribute explanations. The table of contents mirrors the full document; sections that appear missing are simply not needed by players.

---

## 1. Core Mechanics & Attributes

**Three Attributes:** Body, Mind, Soul.  
Range: 0 – 12.  
**Level** = (Body + Mind + Soul) ÷ 3, round down.  
**Attribute Modifier** = Attribute score ÷ 2, round up (e.g. 7 → 4).

| Attribute | Combat Role | Out-of-Combat Role |
|-----------|------------|-------------------|
| **Body** | Max Health, Movement, Mitigation Defense, Melee Attack bonus | Physical feats, endurance, senses, close-quarters intimidation |
| **Mind** | Turn order, Dodge Defense, Ranged Attack bonus | Puzzles, reading people, persuasion, reaction speed |
| **Soul** | Healing Threshold, Known Manifestations/Augments, Arcane Attack bonus | Creativity, luck, empathy, supernatural perception |

---

## 2. Resolution & Checks

### Dice Pool
Your Attribute score determines your dice pool.

| Attribute Points | Dice Pool | Rating |
|------------------|-----------|--------|
| 0 – 4            | 1d6       | Beginner |
| 5 – 8            | 2d6       | Adept |
| 9 – 12           | 3d6       | Expert |

### Reading the Bones
Roll the pool, read each d6 separately.

- **1–3:** 0 Hits
- **4–5:** 1 Hit
- **6:** 1 Hit + **explode** – reroll that die immediately. If the new roll is 4+, gain another Hit. Continue rerolling only as long as you roll 6s.

**Attribute modifiers are not added to dice pools** unless a skill explicitly says so.

### Critical Success
If every die in the pool shows a natural 6 (before any explosions), you earn a **DEVIL** (narrative or mechanical boon, Conductor’s call).

### Difficulty
The Conductor sets a target Hits number.

- **1 Hit:** Standard (basic terminal, sensing a lie)
- **2 Hits:** Hard (master lock, hostile guard)
- **3 Hits:** Heroic (hacking under fire)

### Versus Checks (Contested)
Both parties roll. Compare total Hits.  
Tiebreaker: higher Attribute Modifier.  
If the check is **Derived** (two Attributes), use the highest Modifier of the two for tiebreaking.

### Derived Checks
When an action draws on two Attributes, use the dice pool of the **lower** Attribute score.

| Derived Check | Attributes | Examples |
|---------------|------------|----------|
| **Grit**      | Body + Mind | Stealth, surgery |
| **Aura**      | Body + Soul | Dancing, animal handling |
| **Will**      | Mind + Soul | Deception, insight |

### Attribute Mastery Skills
You may declare only **one** Mastery Skill after rolling.

| Level | Skill         | Effect                                                                                                 |
| ----- | ------------- | ------------------------------------------------------------------------------------------------------ |
| 2     | **Intention** | Exhaust. Reroll any number of 1s.                                                                      |
| 6     | **Precision** | Exhaust. Replace one die with your Attribute Modifier (treat as a die face; if it’s a 6, it explodes). |
| 10    | **Prowess**   | Once per session. Turn one die into a natural 6 (guaranteed Hit + explode).                            |

---

## 3. Combat Structure (The Rhythm)

### Initiative & Turn Order
- PCs act in descending **Mind** attribute order. No roll needed.  
- All enemies act after all PCs, **unless** the Conductor designates a Boss or Miniboss to act at a specific point in PC order (announced before combat).  
- PC ties: the tied players decide order among themselves each round.

### Round Flow
1. **Start of your turn:** Refresh your 2 Full Beats (4 Half-Beats) and your per-round defenses (1 Mitigate, 1 Dodge).  
2. **Surprise (Round 1 only):**  
   - If PCs are ambushed: enemies act first, then PCs.  
   - If enemies are ambushed: PCs act first, enemies lose Swift/Cadence abilities.  
   - Surprised beings cannot use Swift or Cadence.  
3. **End of Round:** Apply pending Status Effect damage/procs, then remove all un-proc’d Status Effects.

### Action Economy (Beats)
At the start of your turn you gain **2 Full Beats** = 4 Half-Beats. Unused Beats are lost.

| Action Type | Cost | Examples |
|-------------|------|----------|
| **Major Action** | 2 HB (1 FB) | Attack (Melee/Ranged), cast a Manifestation, complex skill |
| **Minor Action** | 1 HB | Interact with object, throw item, swap weapons, use item |
| **Free Action** | 0 Beats | Open door, pass through window, speak one short sentence (≈6–8 words) |

**Movement** does not cost Beats. On your turn you have a Movement pool: **Max Movement = 6 + Body attribute**. You may split movement freely between actions. There is no “Dash” action; your pool is your per-turn limit. One tile ≈ 1 meter (or whatever the table agrees).

### Weapon Loadout & Inventory
- You always have **1 Melee** and **1 Ranged** primary weapon equipped. Switching between them is Free.  
- You have 6 inventory slots for additional weapons/tools.  
- Drawing an item from inventory costs 1 HB (Minor Action). Once drawn, it is active until swapped again.  
- No ammo tracking; reloading is Free.  
- No hand restrictions; a greatsword and a sniper rifle can both be primaries.

---

## 4. Movement & Range

**Range Zones** (includes adjacent tiles up to the distance)

| Range | Distance |
|-------|----------|
| Melee | Adjacent tiles only |
| Short | Up to 3 tiles |
| Medium | Up to 6 tiles |
| Long | Up to 9 tiles |
| Very Long | Up to 12 tiles |

**Adjacent** = any tile sharing an edge. (Hex: 6; Square: 8 including diagonals.)

**Fall Damage:** Falls of more than 6 tiles (Medium range) deal 5 Melee damage per additional 3 tiles (Short range). The first 3 tiles of a fall are safe. This damage counts as an Attack Value against you (can be Mitigated or Dodged).

---

## 5. Attack & Defense (The Clash)

### The Attack Sequence
**1. The Attack**  
Attacker rolls: [Dice + Modifiers + Bonuses] = **Attack Value (AV)**.

**2. The Defense**  
Defender chooses one option:

| Option | Cost | Mechanic |
|--------|------|----------|
| **Take It** | Free | Take full damage, no reduction. |
| **Mitigate** | 1 use/round | Subtract your Mitigation Defense Value (MDV) from the incoming damage: `Damage = AV − MDV`. |
| **Dodge** | 1 use/round | Compare your Dodge Defense Value (DDV) to the AV. If DDV > AV, take 0 damage. If DDV ≤ AV, take full damage. |

You regain your 1 Mitigate and 1 Dodge at the start of your turn.

**3. Resolve Damage**  
If final damage ≥ 1 after defenses, subtract from HP. Status Effects and procs only trigger if at least 1 damage gets through.

### Damage Calculation Order
1. Base AV (roll + modifiers)  
2. **Weakness** (attacker side): if defender is Weak to this damage type, AV ×2.  
3. Defender calculates DV.  
4. **Resistance** (defender side): if defender is Resistant, DV ×2.  
5. Status Effect penalties (e.g., Twist: −5 DV).  
6. Compare AV vs DV per defense choice.  
7. Final damage.

### Damage Types
- **Melee / Ranged / Arcane:** standard  
- **Entropy:** cannot be Mitigated or Dodged; Weak/Resistant/Immune apply normally.  
- **Aeon:** true damage; ignores all defenses, resistance, immunity, and reduction.

### Crits
A die showing its natural maximum (e.g., 6 on a d6) is a critical.

- **Precision (single-die weapons):** The rolled value of that die is doubled to the final AV. (e.g., 1d12 crit on a 12 → 24 added before modifiers).  
- **Saturation (multi-die weapons):** Add the weapon’s Chaining Factor (CF) once to the AV.  
- Crits also trigger any “on crit” abilities (e.g., apply Drain).

---

## 6. Special Combat Mechanics

### Targeting Rule
You may target a specific enemy with only **one Attack Sequence** per turn (including Chained attacks and AoE). You can still attack different enemies with separate sequences.

### Defensive Burn (Emergency Defense)
If you’ve used your Mitigate and Dodge for the round and are attacked again, you may Burn:

- **Cost:** Gain 1 Burn Token.  
- **Effect:** Immediately use Mitigate OR Dodge against that attack.  
- **End of your next turn:** Remove all Burn Tokens.  
- **Penalty:** At the start of your next turn, each Burn Token reduces your available Beats by 1 Full Beat (two tokens = 0 Beats).  
- **Limit:** Max 2 Burns per round. No Offensive Burn (no extra attacks).

### Chaining (Combo Attacks)
Combine two attacks into one AV against a single enemy.

1. **Declare:** Pick a Primary Attack (full roll) and a Follow-up Attack (fixed CF).  
2. **Cost:** Sum of both (typically 4 HB total).  
3. **Range:** Both attacks must have matching range, or Ranged at Point Blank can chain with Melee.  
4. **CF:** All attacks list their Chaining Factor. `CF = (Total Maximum Dice Value / 2) – 1` (pre-calculated on equipment).  
5. **Resolution:** Roll Primary normally, then add Follow-up’s CF.  
   `Final AV = Primary Roll + Follow-up CF`.

**Interactions:**  
- Chaining a Manifestation onto a weapon adds CF and may apply additional effects (e.g., Burst).  
- If the chain includes an AoE, the whole sequence becomes that AoE; the second attack’s CF is added to the damage, not repeated.  
- Multi-damage-type chains: if the target is Weak to one type and Resistant to another, the multipliers cancel.

---

## 7. Status Effects & Procs

Status Effects deal Entropy damage and cannot be Mitigated or Dodged (Weak/Resistant/Immune still apply).  
A Being can have one stack of each Status Effect. Applying a second stack **procs** the effect and removes it.

**Duration:** All Status Effects are removed at the end of the afflicted Being’s turn, unless they proc earlier.

| Effect | Standard | PROC |
|--------|----------|------|
| **Burst** (fire/ice/explosion) | At end of turn, take 5 Entropy damage. | **Explosion:** all beings in Short Range take 5 Entropy damage; target takes 10 Entropy damage. Burst removed. |
| **Drain** (bleed/poison/siphon) | Take 5 Entropy damage if you make an Offensive Action or spend Movement. If you do neither, Drain is removed without damage. | **Backlash:** target takes 10 Entropy damage. **Siphon:** attacker heals 5 HP (Overflow). Drain removed. |
| **Twist** (dizzy/confusion) | −5 to all Defense Values (MDV/DDV) until removed. | **Impair:** target’s next Attack Value is −10. **Adrenaline:** attacker gains +5 Movement immediately. Twist removed. |

---

## 8. Fading, Death & Restoration

### Max HP
`10 + 1d4 per Body attribute` (maximum 12d4). Minimum 10, maximum 58, average ~34.

### Fading (HP ≤ 0)
- You have **1 Full Beat** (2 HB) per turn. Cannot Chain.  
- Max Movement = **3 tiles**.  
- Mitigate (1/round) and Dodge (1/round) remain available.  
- **Bleed Out:** At the end of your turn, take 5 Entropy damage.  
- Exit Fading the moment HP is above 0.

### Final Threshold (One-Shot Protection)
If a single attack would reduce your HP from above 0 to **−Max HP or worse**, set HP to `−(Max HP − 1)` instead. This protection refreshes when you heal above 0.

**Single Attack** = one AV (including chains), one AoE instance, or one proc. Multiple separate attacks on the same turn are not covered.

### Stabilization
An adjacent ally may use a Minor Action (1 HB, once per round per target) to negate Bleed Out until you take damage again.

### Death
Permanent death when HP ≤ −Max HP.

### Healing
**Healing Threshold (H.T.)** = 3 + Mind attribute. Total healing you can receive per round from all sources cannot exceed this — unless the healing source has the **Overflow** keyword.

**Out of Combat:** After combat ends, you automatically heal to full HP.

---

## 9. Manifestations & Augments

Manifestations are spells rated Tier I–VI. You may apply **one** Augment per casting.

### Casting Sequence
1. **Declare** Known Manifestation and target.  
2. **Form (Optional):** Choose one Augment (Solid, Liquid, Gas, Plasma).  
3. **Amplify (Optional):** Spend extra Beats to Resonate and add damage dice.  
4. **Create AV:** Roll like a physical attack.

### Costs & Scaling
- Base Half-Beat cost = Tier number (e.g., Tier III = 3 HB).  
- **Minimum cost** 2 HB (reducible via skills).  
- **Resonance (Amplify):** For each additional Half-Beat spent, increase damage by one step: +1 die.  
- **Forced Resonance:** Amplifying beyond your safe limit deals Aeon damage to you equal to the maximum value of every added die.

### Harmonic Resonance Skill
- **Prerequisite:** Soul 2+.  
- **Cost:** 2 MP per level.  
- **Effect:** You may safely Amplify a number of times equal to this skill level.

### Augments (The Forms)

| Augment | Cost | Effect |
|---------|------|--------|
| **Default (Pure Energy)** | Free | Projectile/touch, Medium Range. |
| **Crystallize (Solid)** | +1 HB | Creates tangible object or physical projectile. |
| **Liquify (Fluid)** | +1 HB | Leaves a hazard puddle. |
| **Vaporize (Gas)** | +1 FB | Creates a lingering cloud/mist zone. |
| **Ionize (Plasma)** | +1 FB | Volatile, conductive energy. |

---

## 10. Ability Style Guide (for Players Creating Abilities)

Follow this structure when writing custom abilities.

**Line 1:** [Name] (Beat cost with icon)  
**Line 2:** (Range) (Damage & Damage Type) (Keywords) — omit if not applicable.  
**Effect paragraph:** one block of sentences.  
**Optional:** Flavor quote.

**Beat Cost Icons:**  
- ○ = Free (0 Beats)  
- ◐ = Half-Beat (1 HB)  
- ● = Full Beat (2 HB)  
- ●● = 2 Full Beats (4 HB)

**Writing Rules:**  
- Start every sentence with a concrete verb (Manifest, Grant, Attack, Push, Spend, Create, Teleport…). Never use “You.”  
- No bullet lists inside the effect; a single paragraph of sentences.  
- Use consistent terms: Being, Ally, Enemy, Short Range, etc.  
- An ability with a damage line is an attack; the effect describes what happens on a hit (≥1 damage after defenses).  
- “Perform a free Attack” is only used when granting a brand-new roll (summons, tokens).  
- Use “defeats the target” instead of “reduces to 0 HP”.  
- For repeatable triggers: “Repeatable up to X times.”  
- Keywords like *Exhaust, Combative, Harmless, Swift, Cadence, Overflow* go at the start as fragments.

**Templates:**  
- **Simple Attack:** Attack a Being.  
- **Buff:** Grant an Ally [Benefit] for [Duration].  
- **AoE:** Deal [Amount] [Type] damage to all Beings in [Range].  
- **Manifestation example:**  
  *Firestarter (I) 1HB ◐ (1d4 (CF 1) Arcane) Manifest a spark that applies 🔥Burst. “Its warmth is part of human nature.”*

---

## 11. Mnemonic Skills & Advancement

**Mnemonic Points (MP):** currency for learning skills.  
- +1 MP each time you increase an Attribute.  
- +3 MP per completed Mission/Gig.

### Learning Skills
- **Imprint:** Pay the listed MP cost to learn instantly.  
- **Realize:** Fulfill the unlock condition during play, learn it for free at that moment.

**Notable Skills:**  
- **Apotheosis:** Reduces a chosen Manifestation’s base cost by 1 HB permanently (can be taken multiple times).  
- **Harmonic Resonance** (see Section 9).

### Weapon Upgrades
Weapons have 0–3 upgrade slots.  
- Melee upgrades require Body attribute minimums.  
- Ranged upgrades require Mind attribute minimums.  
(Exact numbers depend on the specific upgrade; consult your weapon sheet.)

---

## 12. Environmental Rules (Downpour)

When rain falls, the Conductor rolls once on the Downpour table at the start of the mission. The effect applies to all combats for the whole mission. Players know which Downpour is active before they commit to action.

| d12 | Effect |
|-----|--------|
| 1   | 1 Beat maximum per turn. |
| 2   | Cannot Chain attacks. |
| 3   | Max Movement halved. |
| 4   | Start each combat with Drain. |
| 5   | All Attack Values halved (round down). |
| 6   | All Defense Values halved (round down). |
| 7   | All CF values halved (round down). |
| 8   | Mitigation unavailable (includes Burn). |
| 9   | Dodge unavailable (includes Burn). |
| 10  | One weapon (your choice) has 0 CF. |
| 11  | No Attribute Modifiers on Attack Values. |
| 12  | All Attack/Defense Values suffer −5 (minimum final value 1). |

---

## 13. Quick Reference

### Action Costs
| Cost | Action |
|------|--------|
| 2 HB (1 FB) | Major Action (Attack, Manifestation) |
| 1 HB | Minor Action (Use Item, Draw Weapon) |
| 0 | Free Action (open door, speak) |
| Movement | Free, pool = 6 + Body |

### Defenses
| Defense | Uses/Round | Effect |
|---------|------------|--------|
| Take It | Unlimited | Full damage |
| Mitigate | 1 | Reduce damage by MDV |
| Dodge | 1 | All or nothing vs AV |
| Burn | Up to 2 (costs Burn Token) | Extra defense, lose Beats next turn |

### Status Effects (Summary)
- **Burst:** 5 Entropy dmg end-of-turn; PROC: AoE 5 dmg, target +5.  
- **Drain:** 5 dmg if move/attack; PROC: 10 dmg + attacker heals 5 Overflow.  
- **Twist:** −5 DV; PROC: target AV −10, attacker +5 Movement.

### Range Bands
| Range     | Distance  |
| --------- | --------- |
| Melee     | Adjacent  |
| Short     | ≤3 tiles  |
| Medium    | ≤6 tiles  |
| Long      | ≤9 tiles  |
| Very Long | ≤12 tiles |