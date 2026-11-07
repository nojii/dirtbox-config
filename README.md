# dirtbox

official config files for the **dirtbox** collection — garry's mod.

drop-in tweaks that clean up the hud, tame a few weapon addons and set up glide vehicles the way they're meant to be played.

---

## what's inside

```
garrysmod/
├── cfg/
│   └── autoexec.cfg   → console tweaks, runs every time the game starts
└── data/
    └── glide.json     → glide vehicle settings + keybinds
```

---

## `autoexec.cfg`

### hud

| command | value | what it does |
| --- | --- | --- |
| `weaponseats_crosshair` | `0` | removes the crosshair while sitting in a vehicle |
| `tacrp_hud` | `0` | hides the tacrp hud |
| `tacrp_minhud` | `0` | hides the tacrp minimal hud |
| `tacrp_drawhud` | `0` | stops tacrp from drawing hud elements |
| `tacrp_hints` | `0` | hides tacrp control hints |
| `ulx showMotd` | `0` | disables the ulx motd popup on join |

### weapons

| command | value | what it does |
| --- | --- | --- |
| `tacrp_autoreload` | `0` | no more automatic reloading on an empty mag |
| `sbox_weapons` | `0` | you spawn with no default weapons |
| `vj_senwepaccuracy_custom` | `1` | sets vj sentry weapon accuracy to 1 |

### binds

| key | command | what it does |
| --- | --- | --- |
| `F11` | `csd_toggle` | blows your brains out |

> `sbox_weapons` and `ulx showMotd` are server-side — they only take effect when you're the one hosting.

---

## `glide.json`

full glide settings file. almost everything is glide's default — the changes are:

| setting | change |
| --- | --- |
| vehicle hud | **off** (`showHUD: false`) |
| horn (cars) | moved to **`F`** |

---

## requirements

the configs only do something if the matching addons are installed — all of them are part of the dirtbox collection:

- **tacrp**
- **vj base** (sentry weapons)
- **ulx**
- **weapon seats**
- **glide**
- the addon that provides `csd_toggle`

---

## installation

1. open your garry's mod folder
   - steam → right-click garry's mod → **manage → browse local files**
2. copy the `garrysmod` folder from this repo over your own and accept the overwrite.
3. restart the game.

> **heads up:** this **replaces** your existing `autoexec.cfg` and glide settings. if you already have stuff in there, back them up first — or just paste the line from `autoexec.cfg` into your own file instead of overwriting it.
