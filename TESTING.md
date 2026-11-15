# Test build notes

All supplied JARs identify themselves as server-side Fabric mods (`environment: server`).

| File | Embedded mod version | Minecraft metadata | Fabric Loader requirement | Fabric API requirement | Java |
|---|---|---|---|---|---|
| `zyns-better-teams-0.2.18+26.1.x.jar` | `0.2.18+26.1.x` | `26.1.x` (manifest: 26.1.2) | `>=0.19.5` | `>=0.155.3` | `>=25` |
| `zyns-better-teams-0.2.16+26.2.jar` | `0.2.16+26.2` | `26.2` | `>=0.19.3` | `>=0.161.0` | `>=25` |
| `zyns-better-teams-0.2.18+26.3.jar` | `0.2.18+26.3` | `26.3` | `>=0.19.5` | `>=0.166.0` | `>=25` |

These values are read from each uploaded JAR's `fabric.mod.json` and manifest. They describe declared metadata, not an independent runtime test report.

## Suggested test checklist

- Fresh dedicated Fabric server starts with the matching JAR.
- First-start configuration is generated.
- Team create, invite, accept, leave, kick, promote, transfer, rename, and disband flows behave as expected.
- Team chat is private to the team.
- Team glow is visible only to teammates when enabled.
- Team data persists after server restart.
- Optional integrations remain inactive when their dependencies are absent.
- Console contains no unexpected exceptions during normal use.

Please include the complete server log and exact game/dependency versions with bug reports.
