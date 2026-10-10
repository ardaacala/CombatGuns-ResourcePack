# CombatGuns Resource Pack

Original weapon visuals and aiming HUD for Minecraft Java Edition **1.21.4**, pack format 46. No client mods required.

[Download current release](https://github.com/ardaacala/CombatGuns-ResourcePack/releases/tag/v1.1.0)

## Server installation

Stop the server, replace the existing `plugins/CombatGuns-1.0.0.jar` with the JAR in the current release, and restart. It configures the official resource-pack URL automatically, including upgrading the previous official v1.0.0 URL. Custom hosting URLs and `resource-pack.auto-configure: false` are preserved.

Players receive the vanilla download prompt when joining. They must accept the updated pack to see the reticles and scope.

## Aiming

Eight distinct weapon reticles, an ammo/reload action bar, and a circular sniper scope. **Left click** with the sniper toggles scope/zoom; **right click** fires; **sneak + right click or Q** reloads. The reticles surround the vanilla center crosshair. HUD graphics use the vanilla title channel while a gun is held; disable `aim-hud.enabled` if another plugin needs exclusive use of titles. The FOV Effects setting affects zoom. Live GUI-scale/alignment and plugin compatibility still require in-game testing.

## Manual hosting configuration

Direct ZIP URL:
https://github.com/ardaacala/CombatGuns-ResourcePack/releases/download/v1.1.0/CombatGuns-ResourcePack.zip

```yaml
resource-pack:
  auto-configure: true
  url: 'https://github.com/ardaacala/CombatGuns-ResourcePack/releases/download/v1.1.0/CombatGuns-ResourcePack.zip'
  sha1: '4ee19dfaee02a56c7e9add2b805f7589768744ee'
  required: false
```

The ZIP need not be copied into the server directory. GitHub hosts the download. The release includes the corresponding plugin JAR for convenience; the pack URL serves only the ZIP.