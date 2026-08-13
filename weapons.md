![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Weapons

Weapons are installed during ship construction.

Each weapon has a fixed **Component Mass**, **Superstructure requirement**, **Total Mass**, **Power Requirement**, **Damage**, and **Range**.

Weapons are purchased individually. They do not use the 1–6 component Rating table unless a weapon rule specifically says otherwise.

---

## Weapon Characteristics

| Characteristic     | Meaning                                                    |
| ------------------ | ---------------------------------------------------------- |
| **Component Mass** | Mass of the weapon itself                                  |
| **Superstructure** | Mass required to mount and support the weapon              |
| **Total Mass**     | Component Mass + Superstructure                            |
| **Power**          | Reactor Power required to fire the weapon once             |
| **Damage**         | Damage caused by a successful hit                          |
| **Range**          | Maximum range band at which the weapon may attack          |
| **MP**             | Movement Points available to the missile each Action Phase |
| **Arc**            | Facings from which the weapon may fire                     |
| **Special**        | Additional rules that apply to the weapon                  |

```text id="dch2e8"
Total Weapon Mass =
Component Mass + Superstructure
```

---

## Missile Launchers

| Weapon                  | Component Mass | Superstructure | Total Mass | Power | Arc  | Special |
| ----------------------- | -------------: | -------------: | ---------: | ----: | ---- | ------- |
| Light Missile Launcher  |              2 |              1 |          3 |     1 | 360° | Missile |
| Medium Missile Launcher |              3 |              2 |          5 |     1 | 360° | Missile |
| Heavy Missile Launcher  |              6 |              3 |          9 |     2 | 360° | Missile |

Missile Launchers fire self-propelled weapons.

Each launch requires the listed Power.

Missiles remain in play after launch and may be intercepted by Point Defense.

Missile Launchers require compatible missiles. Missiles are provisioned through Missile Magazines.

Launcher size determines which missile class it may fire.

```text id="ca9nvx"
Light Missile Launcher  → Light Missile
Medium Missile Launcher → Medium Missile
Heavy Missile Launcher  → Heavy Missile
```

---

## Missiles

Missiles have their own **Range**, **Damage**, and **Movement Point allocation**.

| Missile        | Range | Damage | MP | Compatible Launcher     |
| -------------- | ----: | -----: | -: | ----------------------- |
| Light Missile  |     5 |      4 |  6 | Light Missile Launcher  |
| Medium Missile |     6 |      6 |  4 | Medium Missile Launcher |
| Heavy Missile  |     7 |      9 |  3 | Heavy Missile Launcher  |

**Range** is the maximum range at which the missile may be launched at a target.

**Damage** is the damage inflicted if the missile successfully hits.

**MP** is the number of Movement Points the missile receives during each Action Phase after launch.

Light missiles are faster and more maneuverable.

Medium missiles trade movement for increased range and damage.

Heavy missiles are slower but carry the largest warheads.

### Missile Movement

Missiles use Movement Points in the same general manner as ships unless a missile rule states otherwise.

```text id="smf4eu"
Light Missile  = 6 MP
Medium Missile = 4 MP
Heavy Missile  = 3 MP
```

A missile receives its full MP allocation each Action Phase.

Missile MP does not require additional Reactor Power from the launching ship after launch.

A missile that reaches its target may resolve an attack according to the missile combat rules.

Each Missile Launcher expends one compatible missile when it fires.

```text id="9n6vgy"
1 Missile Launch =
1 Missile expended
```

A Missile Launcher cannot fire if no compatible missile remains aboard the ship.

---

## Missile Magazines

Missile Magazines store missile ammunition.

There are three magazine types:

* Light Missile Magazine
* Medium Missile Magazine
* Heavy Missile Magazine

Each magazine has a fixed ammunition capacity and may only store missiles of its own class.

| Magazine                | Missiles Stored | Component Mass | Superstructure | Total Mass |
| ----------------------- | --------------: | -------------: | -------------: | ---------: |
| Light Missile Magazine  |              12 |              2 |              1 |          3 |
| Medium Missile Magazine |               6 |              2 |              1 |          3 |
| Heavy Missile Magazine  |               3 |              2 |              1 |          3 |

The three magazines have the same Mass and Superstructure requirement.

Larger missiles consume more internal volume, so heavier missile classes store fewer rounds.

```text id="8sexht"
Light Missile Magazine  = 12 Light Missiles
Medium Missile Magazine = 6 Medium Missiles
Heavy Missile Magazine  = 3 Heavy Missiles
```

A ship may install more than one Missile Magazine of any type.

Each additional Magazine adds its full ammunition capacity and its full Mass and Superstructure cost.

Example:

```text id="idohre"
2 Light Missile Magazines

Missiles Stored = 24
Component Mass  = 4
Superstructure  = 2
Total Mass      = 6
```

Multiple compatible Missile Launchers may draw ammunition from the same Missile Magazine.

---

## Missile Summary

| Missile Class | Launcher Total Mass | Launch Power | Magazine Total Mass | Missiles per Magazine | Range | MP | Damage |
| ------------- | ------------------: | -----------: | ------------------: | --------------------: | ----: | -: | -----: |
| Light         |                   3 |            1 |                   3 |                    12 |     5 |  6 |      4 |
| Medium        |                   5 |            1 |                   3 |                     6 |     6 |  4 |      6 |
| Heavy         |                   9 |            2 |                   3 |                     3 |     7 |  3 |      9 |

Light missiles provide the greatest ammunition endurance and highest movement.

Medium missiles trade endurance and movement for increased range and damage.

Heavy missiles provide the greatest individual attack strength, but consume the most launcher Mass, carry the fewest rounds per Magazine, and move the slowest.
