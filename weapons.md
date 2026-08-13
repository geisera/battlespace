![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Weapons

Weapons are installed during ship construction.

Each weapon has a fixed **Component Mass**, **Superstructure requirement**, **Total Mass**, **Power Requirement**, **Damage**, and **Range**.

Weapons are purchased individually. They do not use the 1–6 component Rating table unless a weapon rule specifically says otherwise.

---

## Weapon Characteristics

| Characteristic | Meaning |
| --- | --- |
| **Component Mass** | Mass of the weapon itself |
| **Superstructure** | Mass required to mount and support the weapon |
| **Total Mass** | Component Mass + Superstructure |
| **Power** | Reactor Power required to fire the weapon once |
| **Damage** | Damage caused by a successful hit |
| **Range** | Maximum range band at which the weapon may attack |
| **Arc** | Facings from which the weapon may fire |
| **Special** | Additional rules that apply to the weapon |

```text
Total Weapon Mass =
Component Mass + Superstructure
```

### Missile Launchers

| Weapon | Component Mass | Superstructure | Total Mass | Power | Damage | Range | Arc | Special |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | --- | --- |
| Light Missile Launcher | 2 | 1 | 3 | 1 | 4 | 5 | 360° | Missile |
| Medium Missile Launcher | 3 | 2 | 5 | 1 | 6 | 6 | 360° | Missile |
| Heavy Missile Launcher | 6 | 3 | 9 | 2 | 9 | 7 | 360° | Missile |

Missile Launchers fire self-propelled weapons.

Each launch requires the listed Power.

Missiles may remain in play after launch and may be intercepted by Point Defense.

Missile launchers require missiles to launch. These are provisioned via missile magazines.

### Missile Magazines

Missile Magazines store missile ammunition.

There are three magazine types:

- Light Missile Magazine
- Medium Missile Magazine
- Heavy Missile Magazine

Each magazine has a fixed ammunition capacity and may only store missiles of its own class.

| Magazine | Missiles Stored | Component Mass | Superstructure | Total Mass |
| --- | ---: | ---: | ---: | ---: |
| Light Missile Magazine | 12 | 2 | 1 | 3 |
| Medium Missile Magazine | 6 | 2 | 1 | 3 |
| Heavy Missile Magazine | 3 | 2 | 1 | 3 |

The three magazines have the same Mass and Superstructure requirement.

Larger missiles consume more internal volume, so heavier missile classes store fewer rounds.

```text
Light Missile Magazine  = 12 Light Missiles
Medium Missile Magazine = 6 Medium Missiles
Heavy Missile Magazine  = 3 Heavy Missiles