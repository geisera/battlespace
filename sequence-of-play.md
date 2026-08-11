![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Proposed Sequence of Play

Each game turn is resolved in 6 phases.

### 1. Status Phase

1. Remove expired effects (jams, locks, temporary boosts, etc.).
2. Apply ongoing effects (fires, flooding, reactor strain, crew disruptions).
3. Check scenario timers and victory conditions.

### 2. Allocation Phase

1. Each player secretly allocates reactor power to major systems:
	- Engines
	- Shields
	- Weapons
	- Electronics (ECM/ECCM, sensors, comms)
2. Players may reserve power as capacitor or emergency power, if allowed by ship systems.
3. Record allocations on ship sheets, then reveal simultaneously.

### 3. Initiative Phase

1. Each player determines initiative value using current ship state (command rating, sensor quality, thrust posture, electronic warfare modifiers, damage penalties, etc.).
2. Apply all modifiers and compare totals.
3. Higher total gains initiative for this turn.
4. Tie breaker order:
	- Higher command rating
	- Scenario priority or previous-turn holder (choose one as a standing rule)

### 4. Action Phase A (Initiative Window)

The initiative holder has flexible priority in this phase.

1. Initiative holder chooses one option:
	- Act: declare and resolve one action group.
	- Defer: pass priority to the opposing player without ending participation.
2. Opposing player then chooses one option:
	- Act: declare and resolve one action group.
	- Pass: take no further actions in Phase A.
3. A player who passes is done acting for the rest of Phase A.
4. Phase A ends when both players pass consecutively.

Action group options (choose one per group):

- Maneuver action (vector change, rotation, thrust burst)
- Systems action (reroute, reinforce arc, cooldown, repair order)
- Electronic action (jam, spoof, lock, scan, break lock)
- Weapon action (launch, fire battery, point defense assignment)
- Minor action (crew task, internal prep, decoy deployment)

### 5. Action Phase B (Reaction Window)

The non-initiative player acts first in this phase. No defers are allowed.

1. Non-initiative player declares and resolves one action group.
2. Initiative holder declares and resolves one action group.
3. Continue alternating until both players pass consecutively.

Special rule intent: this phase gives the second player a structured chance to counter and prevents initiative from deciding the entire turn tempo, while avoiding slowdown from repeated defers.

### 6. End Phase

1. Resolve delayed effects triggered at end of turn (arriving missiles, timed detonations, drift-only motion steps, etc.).
2. Update spent power, cooldown tracks, and damage control progress.
3. Clear temporary markers and advance turn counter.

## Table of Contents

* [Sequence of Play](sequence-of-play.md)
* [Maneuver](maneuver.md)
* [Combat](combat.md)
* [Damge](battle-damage.md)
* [Minor Actions](minor-actions.md)
* [Ship Construction](construction.md)
* [Weapons](weapons.md)
* [Auxiliary Equipment](equipment.md)

--- 
