### Keywords

| Keyword       | Meaning                                                                  |
| ------------- | ------------------------------------------------------------------------ |
| **Combative** | Usable only during a combat encounter.                                   |
| **Utility**   | Usable only outside of a combat encounter.                               |
| **Exhaust**   | Usable once per scene or combat encounter.                               |
| **Harmless**  | An ability that does not deal damage.                                    |
| **Overflow**  | Potent healing that bypasses the target’s normal Healing Threshold (HT). |
| **Swift**     | A quick, reactive ability that can be used outside of your turn.         |
| **Cadence**   | Usable only once on each of your turns (once per turn).                  |
| **Passive**   | Active constantly. Requires no Beats.                                    |

---


### Status Effects
All Status Effects deal **Entropy** damage (cannot be Mitigated or Dodged; Weak/Resistant/Immune apply normally).  
A Being can have **one stack** of each effect. Applying a second stack **procs** the effect and removes it.  
All Status Effects are removed at the end of the afflicted Being’s turn, unless they proc earlier.

| Effect                          | Standard                                                                                                                     | PROC                                                                                                                  |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **Burst** (fire/ice/explosion)  | At end of turn, take 5 Entropy damage.                                                                                       | **Explosion:** all Beings in Short Range take 5 Entropy damage; target takes 10 Entropy damage. Burst removed.        |
| **Drain** (bleed/poison/siphon) | Take 5 Entropy damage if you make an Offensive Action or spend Movement. If you do neither, Drain is removed without damage. | **Backlash:** target takes 10 Entropy damage. **Siphon:** attacker heals 5 HP (Overflow). Drain removed.              |
| **Twist** (dizzy/confusion)     | −5 to all Defense Values (MDV/DDV) until removed.                                                                            | **Impair:** target’s next Attack Value is −10. **Adrenaline:** attacker gains +5 Movement immediately. Twist removed. |

---



### Damage Types

| Type        | Special Rules                                                                                                               |
| ----------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Melee**   | Standard physical damage from melee weapons and attacks.                                                                    |
| **Ranged**  | Standard physical damage from ranged weapons and attacks.                                                                   |
| **Arcane**  | Standard magical damage from Manifestations and arcane sources.                                                             |
| **Entropy** | Standard Status Effect or environmental hazard damage. Cannot be Mitigated or Dodged. Weak/Resistant/Immune apply normally. |
| **Aeon**    | True damage. Ignores all defenses, resistance, immunity, and damage reduction.                                              |

---

### Weakness, Resistance & Immunity

Damage calculation follows this order:

1. **Weakness** (attacker side): If defender is **Weak** to the damage type, the Attack Value (AV) is **multiplied by 2**.
2. **Resistance** (defender side): If defender is **Resistant** to the damage type, the Defense Value (DV) is **multiplied by 2**.
3. **Immunity** (defender side): If defender is **Immune** to the damage type, the attack deals **0 damage** (no defenses needed).

> **Cancellation:** If the target is both Weak and Resistant to different damage types in a single attack (e.g., a chain with multiple types), the multipliers cancel — treat as neither Weak nor Resistant.

**Example – Entropy:** Even though Entropy cannot be Mitigated or Dodged, a creature Resistant to Entropy still doubles its DV (though DV is usually irrelevant unless a special defense applies). A creature Immune to Entropy simply takes 0 damage.

**Example – Aeon:** Weakness, Resistance, and Immunity have **no effect** against Aeon damage. It always deals its full AV as damage.