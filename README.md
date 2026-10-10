# CombatGuns — 3D Weapons Resource Pack

Original weapon visuals, 3D held models, animated reloads, muzzle flashes and aiming HUD for **Minecraft Java Edition / Spigot 1.21.4**, Java 21. Vanilla resource pack, no client mods.

[Download the current release](https://github.com/ardaacala/CombatGuns-ResourcePack/releases/tag/v1.2.0)

## Install / update

Stop the server, replace the existing `plugins/CombatGuns-1.0.0.jar` with the JAR from the current release, then restart. The old filename is retained for replacement. The plugin automatically upgrades the old official v1.0.0/v1.1.0 pack URL. Custom URLs and `resource-pack.auto-configure: false` are preserved.

Joining players receive the resource-pack prompt and should accept the update. No ZIP needs to be copied into the server folder. GitHub serves the ZIP directly. Models use namespaced item_model IDs and need the accepted pack to render.

## Visuals and controls

- Eight original inventory/chest icons stay unchanged.
- Held guns use genuine cuboid geometry: receivers, barrels, grips, magazines, stocks and sniper optics.
- Twelve-frame magazine/shell/rocket reloads with slide/bolt/pump movement and eased gun tilt.
- Firing frames show volumetric muzzle flashes and slide/bolt/kick movement; sparse particles accompany the muzzle.
- Item definitions suppress the vanilla re-equip bob on ammunition and model-state updates.
- Eight weapon reticles, an ammo/reload bar and a circular sniper scope.

**Right click** fires. **Sneak + right click or Q** reloads. **Left click with the sniper** opens/closes scope/zoom.

The HUD uses vanilla titles and leaves the vanilla center crosshair intact. FOV Effects affects zoom. Animations are discrete item-model frames, not skeletal player-hand animations. There is no dynamic block lighting. Included 3D previews are offline geometry renders; live hand alignment, GUI scale, FOV, frame timing and compatibility still require in-game testing.

Disable visual animation through `visuals.reload-animation` / `visuals.muzzle-animation`; `aim-hud.enabled` controls the title HUD.

## Manual hosting

```yaml
resource-pack:
  auto-configure: true
  url: 'https://github.com/ardaacala/CombatGuns-ResourcePack/releases/download/v1.2.0/CombatGuns-ResourcePack.zip'
  sha1: '0a750b4dc15be4f42a0bbbd28377802961a3eaa7'
  required: false
```

Pack format 46, Minecraft 1.21.4. Other versions are not verified. Ten tests pass; pack references, 112 3D models and unchanged inventory sprites were validated.