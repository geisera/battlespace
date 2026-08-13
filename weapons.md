![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Weapons

Weapons are installed during ship construction.

Each weapon has a fixed **Component Mass**, **Superstructure requirement**, **Total Mass**, **Power Requirement**, **Damage**, and **Range**.

Weapons are purchased individually. They do not use the 1–6 component Rating table unless a weapon rule specifically says otherwise.

---

## Weapon Characteristics

| Characteristic     | Meaning                                           |
| ------------------ | ------------------------------------------------- |
| **Component Mass** | Mass of the weapon itself                         |
| **Superstructure** | Mass required to mount and support the weapon     |
| **Total Mass**     | Component Mass + Superstructure                   |
| **Power**          | Reactor Power required to fire the weapon once    |
| **Damage**         | Damage caused by a successful hit                 |
| **Range**          | Maximum range band at which the weapon may attack |
| **Arc**            | Facings from which the weapon may fire            |
| **Special**        | Additional rules that apply to the weapon         |

```text
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

Missiles may remain in play after launch and may be intercepted by Point Defense.

Missile Launchers require compatible missiles. Missiles are provisioned through Missile Magazines.

Launcher size determines which missile class it may fire.

```text
Light Missile Launcher  → Light Missile
Medium Missile Launcher → Medium Missile
Heavy Missile Launcher  → Heavy Missile
```

---

## Missiles

Missiles carry their own Range and Damage characteristics.

| Missile        | Range | Damage | Compatible Launcher     |
| -------------- | ----: | -----: | ----------------------- |
| Light Missile  |     5 |      4 | Light Missile Launcher  |
| Medium Missile |     6 |      6 | Medium Missile Launcher |
| Heavy Missile  |     7 |      9 | Heavy Missile Launcher  |

**Range** is the maximum range at which the missile may engage a target.

**Damage** is the damage inflicted if the missile successfully hits.

Larger missiles have greater range and damage, but fewer can be carried in a Magazine.

Each Missile Launcher expends one compatible missile when it fires.

```text
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

```text
Light Missile Magazine  = 12 Light Missiles
Medium Missile Magazine = 6 Medium Missiles
Heavy Missile Magazine  = 3 Heavy Missiles
```

A ship may install more than one Missile Magazine of any type.

Each additional Magazine adds its full ammunition capacity and its full Mass and Superstructure cost.

Example:

```text
2 Light Missile Magazines

Missiles Stored = 24
Component Mass  = 4
Superstructure  = 2
Total Mass      = 6
```

Multiple compatible Missile Launchers may draw ammunition from the same Missile Magazine.

---

## Missile Summary

| Missile Class | Launcher Total Mass | Launch Power | Magazine Total Mass | Missiles per Magazine | Range | Damage |
| ------------- | ------------------: | -----------: | ------------------: | --------------------: | ----: | -----: |
| Light         |                   3 |            1 |                   3 |                    12 |     5 |      4 |
| Medium        |                   5 |            1 |                   3 |                     6 |     6 |      6 |
| Heavy         |                   9 |            2 |                   3 |                     3 |     7 |      9 |

Light missiles provide the greatest ammunition endurance.

Medium missiles trade endurance for increased range and damage.

Heavy missiles provide the greatest individual attack strength, but consume the most launcher Mass and provide the fewest shots per Magazine.
