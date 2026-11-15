# Zyn's Better Teams

A server-side Fabric mod for Minecraft that adds team management features, private team chat, invitations, join requests, aliases, coordinates, colored team-name tags, and optional integrations.

**Project status:** Development is reported complete by the author. These are testing builds; the Modrinth project is not yet published.

## Test builds

| Minecraft target | Mod version | File |
|---|---|---|
| 26.1.x (manifest built against 26.1.2) | 0.2.18+26.1.x | `zyns-better-teams-0.2.18+26.1.x.jar` |
| 26.2 | 0.2.16+26.2 | `zyns-better-teams-0.2.16+26.2.jar` |
| 26.3 | 0.2.18+26.3 | `zyns-better-teams-0.2.18+26.3.jar` |

The JARs are intended for testing on the matching Minecraft target. Do not mix builds across Minecraft versions.

## Requirements

- Fabric Loader (use a release meeting the version requirement in the JAR metadata)
- Java 25 or newer
- The matching Fabric API
- Fabric Permissions API (bundled as a nested dependency in the supplied builds)

Optional integrations suggested by the mod metadata include LuckPerms, TABCore, Placeholder API, and Discord MC Chat. These are not required for basic use.

## Installation

1. Back up your server and world.
2. Install a Fabric server for the exact Minecraft version.
3. Install the matching Fabric API.
4. Put the matching Zyn's Better Teams JAR in the server's `mods/` folder.
5. Start the server and check the console for the mod initialization message.
6. Review `config/zyns-better-teams/config.yml` after the first start and adjust it to your server.

## Testing and feedback

These downloads are supplied for testing, not as a claim that every target has been independently verified on every server setup. Please report the Minecraft version, Fabric Loader version, Fabric API version, full error log, and reproduction steps when reporting a problem. Back up your world before testing.

## Source code

The initial project files available for this upload included the compiled JARs and their embedded metadata/configuration, but not the original Gradle/Java source project. This repository therefore starts with project documentation and test-build information. The original source tree should be added here when it is available; no decompiled code is presented as original source.

## Links

- Portfolio: https://zynayush.github.io/docs/
- Modrinth project page (pending publication): https://modrinth.com/mod/zyns-better-teams

The Modrinth page may not be accessible until moderation and publication are complete.

## License

MIT. See [LICENSE](LICENSE).
