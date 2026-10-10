# CombatGuns Resource Pack

Original weapon textures and item models for CombatGuns on Minecraft Java Edition 1.21.4 (pack format 46). No client mods required.

Download the ZIP from Releases. Server administrators can use this direct URL:

https://github.com/ardaacala/CombatGuns-ResourcePack/releases/download/v1.0.0/CombatGuns-ResourcePack.zip

SHA-1: `1e8c5f91ff849af8061c3a21b709f23cff432437`

In plugins/CombatGuns/config.yml:

```yaml
resource-pack:
  url: 'https://github.com/ardaacala/CombatGuns-ResourcePack/releases/download/v1.0.0/CombatGuns-ResourcePack.zip'
  sha1: '1e8c5f91ff849af8061c3a21b709f23cff432437'
  required: false
```

Restart the server after saving the configuration. Joining players receive the vanilla resource-pack prompt. Set required to true to require acceptance.

This repository distributes the resource pack only. Install the CombatGuns plugin JAR separately in the server plugins folder. The pack does not automatically update the plugin.