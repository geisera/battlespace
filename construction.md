![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Ship Construction

Ships are built in seven steps:

1. Choose Size Class
2. Determine Hull and Structure
3. Install the Reactor
4. Install Propulsion
5. Allocate Armor
6. Install Systems and Weapons
7. Assign Crew and Command

Every choice draws against the same budget: reactor output. Larger hulls demand more power to move, which demands a larger reactor, which feeds larger weapons and heavier armor. A ship is a chain of consequences.

---

### 1. Size Class

Size Class ranges from 1 to 5 and drives every other characteristic.

| Size | Example | Hull Maximum | Structure | Base Signature | Propulsion Cost |
| ---: | --- | ---: | ---: | ---: | ---: |
| 1 | Fighter or shuttle | 12 | 4 | 2 | 1 |
| 2 | Corvette or patrol ship | 24 | 7 | 4 | 1 |
| 3 | Frigate or dropship | 36 | 10 | 6 | 2 |
| 4 | Cruiser | 48 | 13 | 8 | 2 |
| 5 | Battleship or carrier | 60 | 16 | 10 | 3 |

**Propulsion Cost** is the Power required per point of Thrust used in a round. This is the central constraint of construction: a battleship pays three times what a fighter pays to move one point of Thrust.

---

### 2. Hull and Structure

Hull Maximum and Structure are fixed by Size Class.

A ship may trade Hull for capacity. Each 4 points of Hull Maximum removed frees one system slot (see Step 6). Hull Maximum may not be reduced below 8 × Size.

---

### 3. Reactor

Base Reactor Output = **4 × Size Class**.

| Size | Base Output |
| ---: | ---: |
| 1 | 4 |
| 2 | 8 |
| 3 | 12 |
| 4 | 16 |
| 5 | 20 |

A reactor may be upgraded or downgraded at construction:

* **Uprated reactor**: +25% output, rounded down. The reactor occupies one additional system slot and counts as one Size Class larger for critical effect severity.
* **Derated reactor**: −25% output, rounded down. Frees one system slot and reduces Base Signature by 1.

The reactor must produce enough Power to satisfy minimum operating load (see Step 7).

---

### 4. Propulsion

Maximum Thrust = **8 − Size Class**.
Maximum Rotation = **5 − Size Class**, minimum 1.

| Size | Max Thrust | Max Rotation | Power to Use Full Thrust |
| ---: | ---: | ---: | ---: |
| 1 | 7 | 4 | 7 |
| 2 | 6 | 3 | 6 |
| 3 | 5 | 2 | 10 |
| 4 | 4 | 1 | 8 |
| 5 | 3 | 1 | 9 |

Power to use full thrust = Max Thrust × Propulsion Cost. Note that a frigate cannot afford full thrust and full weapons in the same round — its reactor produces 12 and full thrust alone consumes 10. This is intended. Captains choose.

A ship may be built with engines rated below its size maximum. Each point of Thrust below maximum frees one system slot.

**Fuel** = 10 × Size Class + 12. Hard Burn maneuvers consume 2 fuel; all other maneuvers consume 1 fuel per point of Thrust used.

---

### 5. Armor

Armor Budget = **8 + (8 × Size Class)** points, distributed across the four facings.

| Size | Armor Budget | Per-Facing Maximum |
| ---: | ---: | ---: |
| 1 | 16 | 8 |
| 2 | 24 | 10 |
| 3 | 32 | 12 |
| 4 | 40 | 14 |
| 5 | 48 | 16 |

No facing may be left at 0.

Every 8 points of armor installed beyond half the budget increases Base Signature by 1 and reduces Maximum Thrust by 1 (heavy plating slows the ship, demanding still more reactor power per hex of real acceleration).

---

### 6. Systems and Weapons

System Slots = **4 + (2 × Size Class)**.

| Size | System Slots | Weapon Mounts (max) |
| ---: | ---: | ---: |
| 1 | 6 | 2 |
| 2 | 8 | 4 |
| 3 | 10 | 6 |
| 4 | 12 | 8 |
| 5 | 14 | 10 |

The reactor, main engine, and sensor array are mandatory and occupy one slot each. Remaining slots may hold weapons, electronic warfare suites, hangars, shield generators, cargo, or auxiliary equipment.

Each weapon mount occupies one slot. Weapons one class heavier than the ship's Size occupy two slots and may only bear on one firing arc. Weapons two or more classes heavier may not be mounted.

Every installed system lists a **Power Required** value. The sum of Power Required for all systems a captain intends to run simultaneously cannot exceed Reactor Output — a ship may carry more systems than it can power, but something goes dark every round.

---

### 7. Crew and Command

Assign the five crew departments (Command, Engineering, Gunnery, Sensors, Damage Control) skill ratings from 1 to 5. Total department skill points available = **10 + (2 × Size Class)**.

Command Rating may not exceed the Command department's skill.

**Minimum operating load**: Life Support requires 1 Power per Size Class ÷ 2, rounded up (1 Power at Sizes 1–2, 2 Power at Sizes 3–4, 3 Power at Size 5). A reactor unable to meet minimum operating load plus 1 Power of propulsion is not spaceworthy.

---

### Worked Example

**SDC-468 *Archibald Henderson*, Valkyrie-class dropship**

* Size Class 3: Hull 36, Structure 10, Base Signature 6, Propulsion Cost 2
* Standard reactor: Output 12
* Full-rated engines: Thrust 5, Rotation 2 — full thrust costs 10 Power
* Armor: 32-point budget → Fore 10, Aft 6, Port 8, Starboard 8
* Systems: reactor, main engine, sensor array (3 slots), medium coilgun (1 slot), point defense laser (1 slot) — 5 of 10 slots used, remainder given to drop bays
* Fuel: 42
* Crew: 16 skill points across five departments; Command Rating 3

At full burn the *Henderson* has 2 Power left after life support — not enough to fire the coilgun. Her captain either arrives fast or arrives shooting. Not both.

---

## Table of Contents

* [Sequence of Play](sequence-of-play.md)
* [Initiative](initiative.md)
* [Maneuver](maneuver.md)
* [Combat](combat.md)
* [Damge](battle-damage.md)
* [Minor Actions](minor-actions.md)
* [Ship Construction](construction.md)
* [Weapons](weapons.md)
* [Auxiliary Equipment](equipment.md)

--- 
