# SAM Core Ruleset
Welcome to **SAM (Soul Access Memory)**!
This guide contains everything you need to understand the game's core mechanics.
After reading it you should be fully prepared to start playing.

## 1. Your Protagonist’s Core

**Three Attributes:** Body, Mind, Soul. Range: 0 – 12.  
**Level** = (Body + Mind + Soul) ÷ 3, round down.

| Attribute | Combat Role                                                    | Out-of-Combat Role                                             |
| --------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| **Body**  | Max Health, Movement, Mitigation Defense, Melee dice tier      | Physical feats, endurance, senses, close-quarters intimidation |
| **Mind**  | Turn order, Healing Threshold, Dodge Defense, Ranged dice tier | Problem solving, reading people, persuasion, reaction speed    |
| **Soul**  | Manifestations, Augments, Luck Dice                            | Creativity, luck, empathy, supernatural perception             |

---

## 2. Combat

### Action Economy (Beats)
At the start of your turn you gain **4 Beats**. Unused Beats are lost.

| Action Type      | Cost    | Examples                                                                 |
| ---------------- | ------- | ------------------------------------------------------------------------ |
| **Major Action** | 2 Beats | Attack (Melee/Ranged), cast a Manifestation, complex skill               |
| **Minor Action** | 1 Beat  | Interact with object, throw item, swap weapons, use item, stabilize ally |
| **Free Action**  | 0 Beats | Open door, speak one short sentence (≈6–8 words), switch primary weapons |

**Movement** does not cost Beats. Your Movement pool = **6 + Body** tiles per turn. Split movement freely. There is no "Dash" action.

### Initiative & Turn Order
- Protagonists act in descending **Mind** attribute order. No roll needed.  
- All enemies act after all Protagonists, **unless** the Conductor designates a Boss or Miniboss to act at a specific point in Protagonist order (announced before combat).  
- Protagonist ties: the tied players decide order among themselves each round.

### Round Flow
1. **Start of your turn:** Refresh your **4 Beats** and your per-round defenses (1 Mitigate, 1 Dodge).  
2. **Take your turn:** Spend Beats, move, attack.  
3. **End of Round:** Resolve pending Status Effect damage/procs, then remove all un-proc'd Status Effects.

**Surprise (Round 1 only):**
- Surprised beings cannot use Swift or Cadence.  
- If PCs are ambushed: enemies act first, then PCs.

### Example — A Full Turn
*Zoe has Body 5, Mind 7. She starts her turn with 4 Beats, 11 Movement, 1 Mitigate, and 1 Dodge. Two Algiere Soldatos rush her position.*

**Narrative:** Zoe vaults a table (free movement), snaps off a pistol shot at the nearest Soldato, then pivots and drives her knife into the second one before sidestepping into the open lane.

**Mechanical:**
- Move 4 tiles into the room (no Beat cost, 7 Movement remaining).
- Ranged Attack on Soldato A:  Major Action (2 Beats). 
- Spend remaining Beats to Melee Attack Soldato B: Major Action (2 Beats).
- Move 3 tiles into the open lane (free, 4 Movement remaining).
- End of turn. 0 Beats remain.

---

### Weapon Loadout & Inventory
- Always **1 Melee** and **1 Ranged** primary weapon equipped. Switching between them is Free (no Beat cost).  
- 6 Inventory Slots for additional weapons/tools.  
- Drawing from Inventory costs 1 Beat (Minor Action).  
- No ammo tracking; reloading is Free. No hand restrictions.

### Movement & Range
**Range Zones** — includes adjacent tiles up to the listed distance.

| Range | Distance |
|-------|----------|
| Melee | Adjacent tiles only |
| Short | Up to 3 tiles |
| Medium | Up to 6 tiles |
| Long | Up to 9 tiles |
| Very Long | Up to 12 tiles |

**Fall Damage:** Falls of more than 6 tiles deal 5 Melee damage per additional 3 tiles. Counts as an Attack Value (can be Mitigated or Dodged).

---

## 3. Attack & Defense

### Attack Value Formula
```
Attack Value (AV) = Dice Rolls + Weapon Values (+CF for Chaining) 
```

| Component        | Description                                                                |
| ---------------- | -------------------------------------------------------------------------- |
| **Dice Rolls**   | Weapon dice determined by Attribute tier (Body for Melee, Mind for Ranged) |
| **Weapon Bonus** | Weapon quality bonus: Basic +0, Refined +5, Masterpiece +10                |
| **CF**           | Chaining Factor; added just to chain attacks                               |

### The Attack Sequence

**1. The Attack:** Attacker calculates Attack Value (AV).
**2. The Defense:** Defender chooses one:

| Option       | Uses/Round | Mechanic                                                                                            |
| ------------ | ---------- | --------------------------------------------------------------------------------------------------- |
| **Take It**  | Unlimited  | Take full damage.                                                                                   |
| **Mitigate** | 1          | Subtract Mitigation Defense Value (MDV) from damage: `Damage = AV − MDV`.                           |
| **Dodge**    | 1          | Compare Dodge Defense Value (DDV) to AV. If DDV ≥ AV, take 0 damage. If DDV < AV, take full damage. |
(DVs are calculated exactly like AVs but use Armor Bonuses instead.)

Regain 1 Mitigate and 1 Dodge at the start of your turn.

**3. Resolve Damage:** If final damage ≥ 1, subtract from HP. Status Effects, procs, and abilities trigger only if ≥1 damage gets through.

### Example — Defending
*An Algiere Soldato fires a burst from his SMG at Zoe.*

**Scenario A — "Take It"**
Zoe has already used Mitigate on an earlier attack this round and has no Dodge left. She has no choice but to Take It.
- Soldato rolls AV 16. Zoe Takes It. **16 damage** to her HP.

**Scenario B — Mitigate**
Zoe still has her Mitigate available. She rolls with the impact, letting her armor tank the hit.
- Soldato rolls AV 16. Zoe Mitigates: rolls MDV 2d8+2 = `5, 7` + 2 = 14. Damage = 16 − 14 = **2 damage**. A grazing hit.

**Scenario C — Dodge**
Zoe uses her Dodge. She drops low and the burst tears past her shoulder.
- Soldato rolls AV 16. Zoe Dodges: rolls DDV 2d10+2 = `8, 6` + 2 = 16. 16 ≥ 16 → Dodge succeeds. **0 damage**. She rolls to her feet, unharmed.

---

### Damage Types
- **Melee / Ranged / Arcane:** standard  
- **Entropy:** cannot be Mitigated or Dodged; Weak/Resistant/Immune apply normally.  
- **Aeon:** true damage; ignores defenses, resistance, immunity, and reduction.

### Damage Calculation Order
1. Base AV (roll + weapon bonus)
2. **Weakness** (attacker side): if defender is Weak, AV ×2.
3. Defender calculates DV.
4. **Resistance** (defender side): if defender is Resistant, DV ×2.
5. Status Effect penalties (e.g., Twist: −5 DV).
6. Compare AV vs DV per defense choice.
7. Final damage.

### Example — Weakness & Resistance
**Narrative:** She slashes across its exposed wiring, then puts a round into its chest plate point-blank. 

**Mechanical:**
- Primary: Slash sword (2d6, Melee type, 2 Beats). Follow-up: Pistol CF 3 (Ranged type, 2 Beats). Total = 4 Beats.
- Primary roll: 2d6 = `5, 4` = 9. Basic sword (+0) = 9.
- Add follow-up CF: 9 + 3 = **12**. The CF 3 carries Ranged type.
- Chain contains **Melee** (primary) + **Ranged** (follow-up CF).
  - Archivist is Weak to Melee → would double AV.
  - Archivist is Resistant to Ranged → would double DV.
  - Both Weak and Resistant present → **cancellation**. No multipliers.
- Final AV = **12**.
- Archivist Mitigates: rolls MDV 8. Damage = 12 − 8 = **4 damage**.

> **Note:** The CF's damage type is part of the chain. If the Archivist were Weak to Melee with no Ranged Resistance, the full AV would be ×2 = 24. If it were only Resistant to Ranged (no Melee Weakness), the defender's DV would be ×2.

---

### Crits (Explode System)
A Crit occurs when a rolled die shows its **natural maximum value**. All Crit dice **Explode**: roll an extra die of the same type and add it to the total. If that die also shows its maximum, it explodes again, and so on.

When multiple dice crit in the same attack roll, add only **one extra die** total.

**Melee Crits (d6):**
- A natural `6` explodes normally.
- No flat bonus. More consistent crits (16.7% per die).

**Ranged Crits (d8):**
- A natural `8` explodes normally, **and** adds a flat **+5 Lethality Bonus** to the AV.
- More devastating but less frequent crits (12.5% per die).

---

## 4. Special Combat Mechanics

### Targeting Rule
You may target a specific enemy with only **one Attack Sequence** per turn. Once AV − DV is resolved against a Being, you cannot target that Being again this round. You can attack different enemies with separate sequences.

### Example — Targeting
*Three Soldatos surround Zoe. She has 4 Beats and wants to eliminate the leader.*

**Narrative:** She feints toward the leader, forcing him to raise his guard, then pivots and guns down the thug on her left instead. The leader's Mitigate is now wasted, and her ally William has a clear shot.

**Mechanical:**
- Zoe Melee-attacks the leader (2 Beats). The leader Mitigates: his one Mitigate for the round is spent.
- **AV − DV is resolved.** Zoe cannot target the leader again this round.
- Zoe uses her remaining 2 Beats to Ranged-attack a different Soldato.
- Now William's turn. William Chains a Ranged + Manifestation attack against the leader. The leader's Mitigate is already used. He must either Dodge, Take It, or Burn.
- After William resolves AV − DV against the leader, William also cannot target the leader again this round.
- **Result:** Team coordination strips an enemy's defenses across two players' turns.

### Example — Chain Sequence 
Zoe attacks the leader (2 Beats). AV − DV is resolved. She cannot target the leader again this round: the leader is locked for her. She must pick a different target, use an AoE, or end her turn. If she had declared a Chain against the leader as her first attack sequence, the entire chain would count as her one sequence against them.

---

### Chaining (Combo Attacks)
Combine two attacks into one AV against a single enemy.

1. **Declare:** Pick a Primary Attack (full roll) and a Follow-up Attack (fixed CF).  
2. **Cost:** Sum of both costs (typically 4 Beats total).  
3. **Golden Rule:** You may only Chain **two different weapons**, or a weapon and a Manifestation. You **cannot Chain a weapon/Manifestation to itself**.  
4. **Range:** Both attacks must have matching range.
5. **Melee Momentum:** If a Melee weapon is the **Follow-up** (CF-added part), you may instantly move up to **3 tiles** for free between the Primary and the Follow-up to close the distance.  
6. **Resolution:** Roll Primary normally, then add Follow-up's CF. `Final AV = Primary Roll + Follow-up CF`.

**Interactions:**  
- Chaining a Manifestation onto a weapon adds CF and may apply additional effects (e.g., Burst).  
- If the chain includes an AoE, the whole sequence becomes that AoE.  
- The follow-up CF carries its damage type into the chain. The full combined AV (primary roll + follow-up CF) is what Weakness and Resistance apply to.  
- After resolving AV − DV against a Being, you cannot target that Being again this round.

### Example — Weapon + Weapon Chain

*William (Mind 8, Body 5) spots a Bastone enforcer through a shattered window. He draws his Pistol, fires mid-sprint, then drives his Slash knife home.*

**Narrative:** The pistol shot cracks the enforcer's stance. William doesn't stop — he's through the window, knife first.

**Mechanical:**
- Declare: Primary = Refined Pistol (1d8, CF 3, Ranged type, +5 bonus, 2 Beats). Follow-up = Basic Slash knife (2d6, CF 5, Melee type, +0, 2 Beats). Total = 4 Beats.
- Primary roll: 1d8 = `6`. +5 (Refined) = 11.
- Follow-up adds CF 5 (Melee type). Full AV = 11 + 5 = **16**.
- Chain contains Ranged (primary) + Melee (follow-up CF). If the enforcer were Weak or Resistant to either type, apply the rules to the full AV of 16.
- After resolving AV − DV, William cannot target this enforcer again this round.

### Example — Melee Momentum

*William is 4 tiles from a Soldato. He fires his Pistol as the Primary, then uses his Slash knife as the Follow-up to close the gap.*

- Primary: Pistol at range 4 (Medium, OK). Roll as normal.
- Melee Momentum: After the shot, William instantly moves 3 tiles toward the Soldato for free. He's now 1 tiles away: Melee Range. The move brought him adjacent on the grid. CF 5 added.
- **Final AV = Pistol roll + 5.**

---

### Defensive Burn (Emergency Defense)
If you've used both Mitigate and Dodge and are attacked again, you may Burn:

- **Cost:** Gain 1 Burn Token.  
- **Effect:** Immediately use Mitigate OR Dodge against that attack.  
- **End of your next turn:** Remove all Burn Tokens.  
- **Penalty:** At the start of your next turn, each Burn Token reduces your available Beats by **2 Beats** (two tokens = 0 Beats).  
- **Limit:** Max 2 Burns per round. No Offensive Burn.

### Example — Defensive Burn

*Zoe is cornered in the open. She used Mitigate against the first Soldato's burst and Dodge against the second's grenade. A third Soldato levels a rifle at her. She has nothing left.*

**Narrative:** She grits her teeth and throws herself flat as the rifle cracks. The move costs her — she'll be sluggish next turn — but she's alive.

**Mechanical:**
- Zoe has 0 Mitigate and 0 Dodge remaining.
- Third attack incoming. She Burns → gains 1 Burn Token. Uses Mitigate.
- Rolls MDV: 2d8+2 = `6, 4` + 2 = 12. Incoming AV is 18. Damage = 18 − 12 = **6 damage**.
- Next turn: she starts with only 2 Beats instead of 4 (1 Burn Token penalty).
- She could Burn a second time this round (max 2) — but that would leave her with 0 Beats next turn.

---

### Status Effects & Procs
Status Effects deal Entropy damage and cannot be Mitigated or Dodged (Weak/Resistant/Immune still apply).  
A Being can have one stack of each Status Effect. Applying a second stack **procs** the effect and removes it.  
All Status Effects are removed at the end of the afflicted Being's turn, unless they proc earlier.

| Effect                          | Standard                                                                                                                                      | PROC                                                                                                                   |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Burst** (fire/ice/explosion)  | At end of turn, take 5 Entropy damage.                                                                                                       | **Explosion:** all beings in Short Range take 5 Entropy damage; target takes 10 Entropy damage instead. Burst removed. |
| **Drain** (bleed/poison/siphon) | Take 5 Entropy damage whenever you make an Offensive Action or spend Movement. If you do neither, no damage is taken.                          | **Backlash:** target takes 10 Entropy damage. **Siphon:** attacker heals 5 HP (Overflow). Drain removed.               |
| **Twist** (dizzy/confusion)     | −5 to all Defense Values (MDV/DDV) until end of turn.                                                                                         | **Impair:** target's next Attack Value is −10. **Adrenaline:** attacker gains +5 Movement immediately. Twist removed.  |

### Example — Burst PROC

*Zoe manifests Firestarter on a Soldato. Embers dance around his jacket, then catch.*

**Same Round:**
- Zoe's turn: casts Firestarter. Soldato gains 🔥Burst.
- Later in the same round, William casts Firestarter on the Soldato as well. Burst already exists → second stack → **PROC triggers immediately**.
- All beings in Short Range of the Soldato (including his ally next to him) take 5 Entropy damage. The Soldato takes 10 Entropy damage. Burst is removed.
- Soldato's turn: he attacks. At end of turn, no Burst damage — it was already removed by the PROC.
- **Total damage: 10 (target) + 5 (AoE ally) = 15 Entropy.**

**If Zoe had waited instead:**
- Zoe applies Burst (Round 1). Soldato's turn ends → takes 5 Entropy, Burst is removed (end of turn).
- Zoe applies Burst again (Round 2). Soldato's turn ends → takes 5 Entropy, Burst is removed.
- **Total damage: 5 + 5 = 10 Entropy across two rounds.** No PROC. The second application was a fresh stack — Burst had already been cleared.


### Example — Drain Strategy

*A Soldato is afflicted with 🩸Drain. He has a choice.*

- If he attacks or moves: takes 5 Entropy immediately. At end of his turn, Drain is removed (no further damage).
- If he does nothing: no damage is taken. At end of his turn, Drain is removed without triggering.
- Either way, Drain is gone by the end of his turn: the question is whether he pays 5 Entropy to act, or gives up his turn to survive.

---

## 5. Manifestations & Augments

Manifestations are spells rated Tier I–VI. You may apply **one** Augment per casting.

### Casting Sequence
1. **Declare** Known Manifestation and target.  
2. **Form (Optional):** Choose one Augment (Solid, Liquid, Gas, Plasma).  
3. **Amplify (Optional):** Spend extra Beats to Resonate and add damage dice.  
4. **Create AV:** Roll like a physical attack.

### Costs & Scaling
- Base Beat cost = Tier number (e.g., Tier III = 3 Beats).  
- **Minimum cost** 2 Beats (reducible via skills).  
- **Resonance (Amplify):** For each additional Beat spent, increase damage by one step: +1 die.  
- **Forced Resonance:** Amplifying beyond your safe limit deals Aeon damage to you equal to the maximum value of every added die.

### Example — Safe Amplify

*Veyra (Soul 5, Harmonic Resonance 2) corners a Machina Scraper in an alley. She casts Psy Knife (Tier II, base 2d6) and pours extra power into it.*

**Narrative:** The neon-pink stiletto of psychic force materializes above her palm — then doubles, triples in intensity. She drives it through the Scraper's chassis with a scream.

**Mechanical:**
- Base cost: 2 Beats (Tier II). Base dice: 2d6.
- Amplify twice: +2 Beats. Total 4 Beats. Adds +2 dice → rolls **4d6**.
- Harmonic Resonance skill is 2, Amplifying 2 times is safe. No self-damage.
- Roll 4d6 = `5, 3, 6, 2` = 16.
- Total AV = 16 + CF 2 (if the manifestation lists one).

### Example — Forced Resonance

*Desperate, Veyra pushes beyond her limit. She pours everything into the spell — and her own body pays the price.*

**Narrative:** The stiletto becomes blinding — too bright to look at. Cracks of black energy crawl up her arm as the excess power feeds back. She releases it anyway.

**Mechanical:**
- Same Tier II Manifestation (2d6). Amplify **3** times: +3 Beats, total 5 Beats.
- Harmonic Resonance skill is 2. The third Amplify exceeds the safe limit.
- Rolls 5d6 for damage. But also takes Aeon damage equal to the maximum value of that third extra die = **6 Aeon damage to herself**.
- She can keep Amplifying further, but each additional die beyond her limit deals another 6 Aeon damage.

---

### Harmonic Resonance Skill
- **Prerequisite:** Soul 2+.  
- **Cost:** 2 MP per level.  
- **Effect:** You may safely Amplify a number of times equal to this skill level.

### Augments (The Forms)

| Augment | Cost | Effect |
|---------|------|--------|
| **Default (Pure Energy)** | Free | Projectile/touch, Medium Range. |
| **Crystallize (Solid)** | +1 Beat | Creates tangible object or physical projectile. |
| **Liquify (Fluid)** | +1 Beat | Leaves a hazard puddle. |
| **Vaporize (Gas)** | +2 Beats | Creates a lingering cloud/mist zone. |
| **Ionize (Plasma)** | +2 Beats | Volatile, conductive energy. |

---

## 6. Survival

### Max HP
`10 + 1d4 per Body attribute` (maximum 12d4). Minimum 10, maximum 58, average ~34.

### Fading (HP ≤ 0)
When you hit 0 HP or below, you enter Fading.

- **The Timer:** Gain 1 Fading Token at the start of your turn. At **3 Fading Tokens**, you die permanently.
- **Limitations:** 2 Beats per turn. Max Movement 3 tiles. Cannot Chain.
- **Stabilize:** Cadence. An Ally in Short Range may spend **1 Beat** to remove 1 Fading Token.
- Exit Fading the moment your HP rises above 0, clearing all tokens.


### Example — Fading

*Zoe takes a grenade to the chest. The world goes muffled. She's on her back, looking at the ceiling, and everything hurts twice as much.*

**Turn-by-turn:**
- **Hit:** AV 22. Zoe's at 8 HP. 8 − 22 = −14. She enters Fading.
- **Turn 1:** Gain Token 1 (2 remaining until death). Zoe has 2 Beats, 3 Movement. She crawls 3 tiles toward William. An enemy shoots her for 6 → doubled to **12 damage** (−26 HP).
- **Turn 2:** Gain Token 2 (1 remaining). William is adjacent now. He spends 1 Beat to Stabilize → removes 1 Fading Token (back to Token 1). William then heals her with Faint Smile for 8 HP (−18 HP, still Fading).
- **Turn 3:** Gain Token 2 again. Another ally heals for 10 HP (−8 HP, still Fading).
- **Turn 4:** Gain Token 3 — **Zoe dies.** She was never healed above 0.

**What should have happened:** If William had healed her above 0 on Turn 2 or 3 (e.g., two big heals instead of one), she'd exit Fading and clear all tokens. She'd be back in the fight.

### Mortal Reminder (−Max HP Rule)
You no longer die instantly at −Max HP. However, if your HP drops to −Max HP or lower, you sustain a **Mortal Reminder**. You survive the fight, but your sense of Self is broken.

- **The Debuff:** Begin all subsequent combats at exactly **1 HP**.
- **The Cure:** Mortal Reminder can only be cleared by administering a **Trauma Kit** (a rare, specialized consumable item).

### Example — Mortal Reminder

*Zoe has 25 Max HP. During a boss fight, a direct hit drops her from 10 HP to −28 HP — past her −Max HP threshold. She doesn't die. She wakes up after the fight, but something is wrong.*

- Her sense of self is fractured. In every combat from now on, she starts at **1 HP** — regardless of her actual Max HP.
- Manifestations and standard healing cannot fix this. Only a **Trauma Kit** can restore her.
- The crew now has a new mission: find a Trauma Kit before the next big gig.

---

### Healing
**Healing Threshold (H.T.)** = 3 + Mind attribute. Total healing you can receive per round from all sources cannot exceed this — unless the healing source has the **Overflow** keyword.

**Out of Combat:** After combat ends, you automatically heal to full HP.

### Example — Healing Threshold

*Zoe (Mind 4, HT = 7) takes a bad hit. Two allies try to patch her up.*

- William casts Faint Smile: heals 9 HP. But HT is 7, so only **7 HP is restored** (the remaining 2 is wasted).
- If William's Faint Smile had **Overflow**, all 9 HP would go through — bypassing the HT cap entirely.
- A second ally tries to heal her in the same round. HT has already been reached — 0 additional healing unless Overflow.
- **Next round:** HT resets. She can be healed again.

---

## 7. Skill Checks

### Dice Pool
Your Attribute score determines your dice pool.

| Attribute Points | Dice Pool | Rating |
|------------------|-----------|--------|
| 0 – 4 | 1d6 | Beginner |
| 5 – 8 | 2d6 | Adept |
| 9 – 12 | 3d6 | Expert |

### Reading the Bones
Roll the pool, read each d6 separately.

- **1–3:** 0 Hits
- **4–5:** 1 Hit
- **6:** 1 Hit + **explode** – reroll that die immediately. If the new roll is 4+, gain another Hit. Continue rerolling only as long as you roll 6s.

**Attribute modifiers are not added to dice pools** unless a skill explicitly says so.

### Example — Skill Check

*William (Body 7 → 2d6 pool) attempts to parkour across a collapsing catwalk in the Glassgrave district. The Conductor calls for a Body check, difficulty 2 Hits.*

- Roll 2d6 = `4, 6`. The `4` = 1 Hit. The `6` = 1 Hit + explodes.
- Explosion: roll extra d6 = `3` (3 is below 4, no extra Hit).
- Total Hits = 2. The difficulty was 2. **Success.** William clears the gap as the catwalk buckles behind him.

**If he'd rolled `3, 5`:** 0 + 1 = 1 Hit. **Failure.** The catwalk gives way — William plummets, taking fall damage, and now the crew has a rescue problem.

---

### Critical Success
If every die in the pool shows a natural 6 (before any explosions), you earn a **DEVIL:** until the end of the current session, you may change one specific detail. As long as it's not too outrageous, the Conductor should allow it.

### Difficulty
The Conductor sets a target Hits number.

- **1 Hit:** Easy (basic terminal, sensing a lie)
- **2 Hits:** Medium (master lock, hostile guard)
- **3 Hits:** Hard (hacking under fire)
- 4+ Hits are used very rarely as they become extremely hard.

### Versus Checks (Clashes)
Both parties roll. Compare total Hits.  
Tiebreaker: higher Attribute.  
If the check is **Derived** (two Attributes), use the highest Attribute of the two for tiebreaking.

### Derived Checks
When an action draws on two Attributes, average them: **(Attribute1 + Attribute2) ÷ 2**, rounded down. Use the dice pool for that resulting score.

> **Note:** Normally this would already be written on you character sheet, so no math would be needed.

| Derived Check | Attributes | Examples |
| ------------- | ----------- | ------------------------ |
| **Grit** | Body + Mind | Stealth, crafting |
| **Aura** | Body + Soul | Dancing, animal handling |
| **Will** | Mind + Soul | Deception, insight |

### Example — Derived Check (Grit)

*Zoe (Body 7, Mind 4) needs to sneak past a Machina patrol drone. This is a Grit check (Body + Mind) — physical control plus mental focus.*

- Average: (7 + 4) ÷ 2 = 5.5 → rounded down to **5**.
- Attribute 5 grants a **2d6** dice pool.
- Roll 2d6 = `4, 3`. 1 Hit. The Conductor set difficulty at 1 Hit. **Success.** She slips past the drone's scanner.
- If she'd had Mind 2 (7+2=9÷2=4 → 1d6), her low mental focus would drag her down despite her athleticism.

---

### Attribute Mastery Skills
You may declare only **one** Mastery Skill after rolling.

| Level | Skill | Effect |
| ----- | ------------- | --------------------------------------------------------------------------- |
| 2 | **Intention** | Exhaust. Reroll any number of 1s. |
| 6 | **Precision** | Exhaust. Replace one die with 5 (guaranteed Hit). |
| 10 | **Prowess** | Once per session. Turn one die into a natural 6 (guaranteed Hit + explode). |

---

## 8. Advancement

**Mnemonic Points (MP):** currency for learning skills.  
- +1 MP each time you increase an Attribute.  
- +3 MP per completed Mission/Gig.

### Learning Skills
- **Imprint:** Pay the listed MP cost to learn instantly.  
- **Realize:** Fulfill the unlock condition during play, learn it for free at that moment.

**Notable Skills:**  
- **Apotheosis:** Reduces a chosen Manifestation's base cost by 1 Beat permanently (can be taken multiple times).  
- **Harmonic Resonance** (see Section 5).

### Weapon Upgrades
Weapons gain upgrade slots based on quality. Melee upgrades require **Body** minimums; Ranged upgrades require **Mind** minimums.  
Upgrades can be equipped on weapons at any time, but using them requires the specific skills. Unless stated otherwise, Upgrades can be changed from one weapon to another freely.

---

## 9. Quick Reference

### Action Costs
| Cost | Action |
|------|--------|
| 2 Beats | Major Action (Attack, Manifestation) |
| 1 Beat | Minor Action (Use Item, Draw Weapon, Stabilize) |
| 0 | Free Action (open door, speak) |
| Movement | Free, pool = 6 + Body |

### Attack Value
`AV = Dice Rolls + Weapon Values + CF`

### Defenses
| Defense | Uses/Round | Effect |
| -------- | -------------------------- | ----------------------------------- |
| Take It | Unlimited | Full damage |
| Mitigate | 1 | Reduce damage by MDV |
| Dodge | 1 | All or nothing vs AV |
| Burn | Up to 2 (costs Burn Token) | Extra defense, lose 2 Beats next turn per token |

### Crits
| Type            | Trigger   | Effect                                           |
| --------------- | --------- | ------------------------------------------------ |
| **Melee** (d6)  | Natural 6 | Explode (add d6, repeat on 6)                    |
| **Ranged** (d8) | Natural 8 | Explode (add d8, repeat on 8) + **+5 Lethality** |

- **Burst:** 5 Entropy dmg end-of-turn; PROC: AoE 5 dmg, target +5.  
- **Drain:** 5 dmg if move/attack; PROC: 10 dmg + attacker heals 5 Overflow.  
- **Twist:** −5 DV; PROC: target AV −10, attacker +5 Movement.

### Range Bands
| Range | Distance |
| --------- | --------- |
| Melee | Adjacent |
| Short | ≤3 tiles |
| Medium | ≤6 tiles |
| Long | ≤9 tiles |
| Very Long | ≤12 tiles |

### Fading Quick Reference
| Step | Effect |
|------|--------|
| Enter | HP ≤ 0 |
| Tokens | +1 per turn; die at 3 tokens |
| Penalty | Double damage taken, 2 Beats, 3 Mov, no Chain |
| Stabilize | Ally spends 1 Beat, removes 1 token |
| Exit | HP > 0, clear all tokens |
| Mortal Reminder | HP ≤ −Max HP → start future combats at 1 HP (Trauma Kit cure) |
