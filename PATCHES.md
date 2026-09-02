# Main Server Patch History

This document records the history of the required client patch set used by the server.

The history has been reconstructed from the archived `patch-V.mpq` and `patch-Z.mpq` releases, the DBC files stored alongside them, saved working files, and Individual Progression update resources.

Where a loose working file existed but was not present inside the finished MPQ, it is treated as development work rather than a released change.

## Main Patch Files

The required client patch set is primarily split between:

- `patch-V.mpq` — client data including spells, items, skills, achievements and flight-path data.
- `patch-Z.mpq` — primarily `ItemExtendedCost.dbc`, used for custom vendor purchase requirements.

These are **Main Server Patches** and are separate from optional cosmetic or personal client patches.

---

## Patch 1.0.1 — Initial Main Server Patch

The first preserved version of the required client patch set and the baseline used for all later comparisons.

`patch-V.mpq` already contained custom client data for achievements, items, skills, spells and flight paths. `patch-Z.mpq` contained the custom ExtendedCost data used by server vendors.

Because this is the earliest archived release, changes made before 1.0.1 cannot be reliably separated from the baseline.

---

## Patch 1.0.2

### Maintenance

- Repacked `patch-Z.mpq`.
- No actual `ItemExtendedCost.dbc` gameplay-data changes were found compared with 1.0.1.

This appears to have been a packaging/maintenance update rather than a gameplay update.

---

## Patch 1.0.3

### Bird of Prey Pet Abilities

- Added the missing Bird of Prey pet ability ranks to `SkillLineAbility.dbc`.
- Completed the Bird of Prey ability progression beyond the first rank.

Technical records added: `21981–21985`.

---

## Patch 1.0.4

### TBC PvP Vendor Costs

- Added 48 new ExtendedCost records.
- Added client support for the TBC-style PvP purchasing system using **Honor together with battleground marks**.

This aligned the client with the PvP vendor costs being used by the server and Individual Progression.

---

## Patch 1.0.4 — Hot Fix

### PvP Vendor Fix

- Removed ExtendedCost records `4000–4012`.
- Removed the conflicting Honor-only cost block while retaining the larger Honor + battleground-mark system introduced in 1.0.4.

---

# 1.0.5 Series

## Patch 1.0.5

### Realm First Level Achievements

Added two custom maximum-level achievements:

- **Realm First! Level 70** — Achievement `6250`
- **Realm First! Level 60** — Achievement `6255`

Matching level criteria were also added.

### Battleground and Custom Spell Support

Added the first large custom client spell block used by the server, including battleground-only effects for movement speed, Rage, Energy, stealth detection, sharpening/weighting effects and test healing support.

This version also introduced the initial custom Strong Troll's Blood Elixir effect.

### Custom Item Support

- Added client item records `60100–60109`.

### Older-Expansion Mana Costs

Adjusted several spells/forms toward their older-expansion percentage mana costs, including:

- Lay on Hands
- Cat Form
- Travel Form
- Aquatic Form
- Bear Form
- Dire Bear Form
- Moonkin Form
- Power Word: Fortitude

### Holiday Vendor Costs

Added client purchase-cost support for multiple seasonal event currencies:

- **Love Token** — 15 / 35 / 50 / 100
- **Lovely Charm Bracelet** — 5
- **Coin of Ancestry** — 10 / 15 / 20
- **Noblegarden Chocolate** — 125 / 150 / 175 / 200 / 225 / 250

---

## Patch 1.0.5.1

### Crowe's Elixirs

Introduced the first custom Crowe healing and mana effect spells.

Four effect records were added across the custom `81000` spell range.

### Spell Duration Support

- Added `SpellDuration.dbc` to the main patch set to support the custom duration behaviour being introduced.

---

## Patch 1.0.5.2

### Crowe's Elixir Refinement

- Renamed the primary healing effect to **Crowe's Healing Elixir Effect**.
- Renamed the primary mana effect to **Crowe's Mana Elixir Effect**.
- Refined the duration references used by both effects.

---

## Patch 1.0.5.3

### Maintenance / Development Build

No released DBC changes were found compared with 1.0.5.2.

A newer loose `Item.dbc` existed in the working folder, but those experimental item changes were not packed into the released MPQ and are therefore not counted as release changes.

---

## Patch 1.0.5.4

### Battleground Injectors

Added custom effects for:

- **Battleground Health Injector**
- **Battleground Mana Injector**
- **Battleground Health & Mana Injector**

The Crowe healing and mana regeneration effects were also refined further.

### Custom Items

Added client records:

`59991`, `59992`, `59995`, `59996`, `59997`, `59998`, `59999`.

---

## Patch 1.0.5.5

### Warlock Armour Restoration

Restored `Demon Skin` and `Demon Armor` toward their older health-regeneration behaviour.

- Replaced the later increased-healing-received behaviour with passive health regeneration data.
- Restored periodic regeneration behaviour.
- Updated the related client descriptions.

---

## Patch 1.0.5.6 — Individual Progression Update

### Individual Progression Spell Refresh

Rebuilt `Spell.dbc` from the newer Individual Progression spell data while preserving the server's custom spell work.

The finished file is the IP-provided Spell data with the existing custom server spell records added back on top. No existing IP spell records were overwritten during this particular merge.

This preserved the Crowe effects, battleground consumables and other custom spell work already present on the server.

---

## Patch 1.0.5.7.1 — Hot Fix

### Hearthstone

- Changed the Hearthstone cooldown from **30 minutes to 60 minutes**.

### Custom Items

Added client item records:

- `60095`
- `60096`

---

## Patch 1.0.5.8

### Hearthstone

- Changed the Hearthstone cooldown from **60 minutes back to 30 minutes**.

No additional released Item data change occurred in this version.

---

## Patch 1.0.5.9

### Hearthstone

- Changed the Hearthstone cooldown from **30 minutes back to 60 minutes**.

### Development Note

Server-specific loading-tip work was also being developed around this version, but the edited `GameTips.dbc` was not included in the finished MPQ and is therefore not treated as a released feature.

---

## Patch 1.0.5.9.1

### Maintenance / Checkpoint Build

No verified released client-data change was found for this version.

The saved Map work and bundled MPQs are effectively carry-forwards of the existing patch data, so this appears to have been a working/version checkpoint.

---

# 1.0.6 Series

## Patch 1.0.6.0 — Individual Progression Update

### Item Enchantment Client Data

- Added `SpellItemEnchantment.dbc` to the main client patch set.

### Spell Data

The `Spell.dbc` actually shipped in this version remained unchanged from 1.0.5.9, despite newer IP Spell data being present in the update resources.

A historical review item relating to two IP enchant records from this update is recorded near the bottom of this document.

---

## Trial Patch 1.0.6.1

### Khadgar's Unlocking Experiment

Trialled a revised four-rank progression for the existing **Khadgar's Unlocking** chain:

- Rank 1 — Spell `491`
- Rank 2 — Spell `857`
- Rank 3 — Spell `10165`
- Rank 4 — Spell `10166`

The trial adjusted cast-time data, level requirements, unlocking strength, mana cost and Mage spell-class data.

This was a testing build rather than a normal stable release.

---

## Patch 1.0.6.2 — Individual Progression Update

### Individual Progression Spell Merge

Merged the newer Individual Progression Spell data while selectively preserving the server's custom systems.

The merge preserved:

- Core battleground utility effects.
- Crowe's custom healing and mana effects.
- Battleground injector effects.
- The Khadgar's Unlocking trial changes.
- The 60-minute Hearthstone cooldown.

The old custom spell using ID `81000` was not retained because Individual Progression had begun using that ID itself. The temporary sharpening/dynamite spell block at `81504–81509` was also not re-added.

### Item Data Rebuild

`Item.dbc` was rebuilt around the updated data and a deliberately curated custom-record list.

This preserved the custom records that were still required by the server while dropping older records that were no longer carried into the rebuilt Item data.

---

## Patch 1.0.6.3

### Priest — Sleep

Updated **Sleep** (`700`):

- Maximum target level changed from **30 to 60**.
- Fixed mana cost changed from **60 to 120**.
- Added the revised percentage mana-cost data used by this version.
- Updated the client tooltip threshold to level 60.

### Priest Holy Skill Data

Added a new `SkillLineAbility` record linking **Sleep** to the **Priest Holy** skill line.

### Development Work Not Released

Two loose working files were present in the version folder but were not included in the released MPQ:

- `GameTips.dbc`
- `LFGDungeons.dbc`

These are kept as development history rather than release changes.

---

## Patch 1.0.6.4 — Minor Patch

### Restored Client Item Records

Added 17 `Item.dbc` records:

`65–75`, `160–163`, `166`, `167`.

No existing Item records were altered by this minor update.

---

## Patch 1.0.6.5

### Khadgar's Unlocking

Formally connected **Khadgar's Unlocking (Rank 1)** to the Mage **Arcane** skill line.

### Flight Path Economy

Performed a large flight-path price rebalance.

- **767 flight routes** changed.
- **763 routes** were increased to approximately **5.5×** their previous cost.
- The Stormwind ↔ Ironforge and Thunder Bluff ↔ Orgrimmar capital routes received larger manual prices.

---

## Patch 1.0.6.6 — Individual Progression Update

### Tiny Bronze Key

- Corrected the client display ID for **Tiny Bronze Key (5517)**.

### Individual Progression Spell Refresh

The new IP Spell data introduced 44 meaningful spell-data changes.

#### Sleep

Sleep was returned to the lower-level version used by the updated IP data:

- Maximum target level returned from 60 to 30.
- Mana cost returned from 120 to 60.
- The tooltip threshold returned to level 30.

#### Earth Shock

Seven ranks of Earth Shock were restored from attack-speed-reduction behaviour to their interrupt/school-lockout behaviour.

#### Fixed Mana Costs

A large group of level-60/70-era spells were restored from percentage-based mana costs to fixed older-expansion mana costs.

Affected classes include Priest, Shaman, Druid, Mage, Paladin and Warlock.

### Extended Costs

`patch-Z.mpq` was repacked, but its actual ExtendedCost gameplay data remained unchanged.

### Server Item Stack Sizes

The accompanying server update also restored/rebalanced many item stack sizes toward Vanilla-style values across materials, consumables and other items.

---

## Patch 1.0.6.7 — Individual Progression Update

### Individual Progression Spell Refresh

The final `Spell.dbc` was refreshed directly from the latest Individual Progression data.

Between 1.0.6.6 and 1.0.6.7, every other DBC inside `patch-V.mpq` remained unchanged and `patch-Z.mpq` was unchanged.

### Holy Light

**Holy Light (647)** changed from a **34% mana cost** to a fixed **110 mana** cost.

### Individual Progression / Server Fixes

This release was accompanied by several server-side Individual Progression and event fixes:

- Refreshed Individual Progression Spell data.
- Corrected the Horde Paladin mount quest chain.
- Restored the original scripted Brewfest mount purchasing system.
- Restored quest-completion checks for Brewfest mount vendors.
- Restored the relevant Brewfest mounts and their pricing.
- Restored access to the required quest through the token-redeemer system.
- Rebalanced the Hallow's End village-fire event for smaller groups.
- Reduced the difficulty of the Brewfest Dark Iron attack event.

---

# Development and Historical Notes

## Working Files vs Released MPQs

Some archived version folders contain loose DBC files, backups, experiments or editor exports that were never packed into the finished release.

These have deliberately been kept out of the main patch notes unless they help explain how a later feature developed.

Examples include:

- Experimental Item work in 1.0.5.3.
- Server-specific `GameTips.dbc` work around the late 1.0.5 / early 1.0.6 period.
- `LFGDungeons.dbc` work in 1.0.6.3.

## Historical IP Merge Review

One unresolved historical difference remains worth checking.

The Individual Progression `SpellItemEnchantment.dbc` resource used during the 1.0.6.0 update contained two additional enchantment records:

- `4001` — **+30 Healing Spells and +10 Damage Spells**
- `4003` — **+35 Healing Spells and +12 Damage Spells**

These two records were not included in the server's finished `SpellItemEnchantment.dbc` and remain absent in the current 1.0.6.7 patch.

This is recorded as a **review item**, not a confirmed bug, because the archived files prove the difference but do not prove whether the omission was intentional.

---

# Current Main Patch

The latest archived Main Server Patch covered by this history is:

**Patch 1.0.6.7 — Individual Progression Update**

The current required client patch set uses:

- `patch-V.mpq`
- `patch-Z.mpq`
