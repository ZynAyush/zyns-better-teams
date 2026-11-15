# Compatibility

Zyn's Better Teams is a server-side Fabric mod. Install the build that matches the Minecraft server version exactly. A client-side installation is not required for players.

| Minecraft version | Mod version | Compiled against | Fabric Loader | Fabric API | Java |
|---|---|---|---|---|---|
| 26.1.x | 0.2.18+26.1.x | 26.1.2 | 0.19.5+ | 0.155.3+26.1.2 | 25+ |
| 26.2 | 0.2.16+26.2 | 26.2 | 0.19.3+ | 0.161.0+26.2 | 25+ |
| 26.3 | 0.2.18+26.3 | 26.3 | 0.19.5+ | 0.166.0+26.3 | 25+ |

## Required

- Fabric dedicated server for the target Minecraft version
- Matching Fabric Loader
- Matching Fabric API
- Java 25 or newer

## Optional

- Placeholder API for placeholder expansion
- LuckPerms for permission integration
- TABCore for supported TAB integration
- Discord webhook configuration for outbound event notifications

Fabric Permissions API is bundled in the mod JAR. Do not install a second copy unless the server's dependency resolution requires it.

## Notes

- Do not mix JARs between Minecraft target versions.
- Back up the world and configuration before updating.
- This is a test-build project; compatibility should be verified on a staging server before use on a production world.
