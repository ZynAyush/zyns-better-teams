# Zyn's Better Teams

A server-side Fabric mod for managing persistent player teams in Minecraft. Players can use the mod's team features without installing it on their own clients.

> **Project status:** Development is complete. Test builds are prepared for Minecraft 26.1.x, 26.2 and 26.3. The Modrinth project page is awaiting moderation; GitHub is the project source of truth while that review is pending.

## Features

- Create, rename, transfer and disband teams.
- Invite players, manage join requests, accept or decline invitations, and manage team members.
- Switch between global chat and team-only chat.
- Set team label colours and friendly-fire preferences.
- View teammate coordinates and create personal aliases for teammates.
- Toggle the vanilla glowing outline for team members.
- Configure messages, limits and behavior through YAML configuration.
- Optional integrations for LuckPerms, Placeholder API, TABCore and Discord webhooks where supported.

## Compatibility

| Minecraft | Mod version | Fabric Loader | Fabric API | Java |
|---|---|---|---|---|
| 26.1.x (compile target 26.1.2) | 0.2.18+26.1.x | 0.19.5+ | 0.155.3+26.1.2 | 25+ |
| 26.2 | 0.2.16+26.2 | 0.19.3+ | 0.161.0+26.2 | 25+ |
| 26.3 | 0.2.18+26.3 | 0.19.5+ | 0.166.0+26.3 | 25+ |

Use the JAR and Fabric API matching the server's exact Minecraft version. Fabric Permissions API is bundled in the mod JAR. Placeholder API is optional.

## Installation

1. Back up the server and world.
2. Install a Fabric dedicated server for the matching Minecraft version.
3. Install the matching Fabric API.
4. Put the matching Zyn's Better Teams JAR in the server's `mods/` folder.
5. Start the server and review `config/zyns-better-teams/config.yml`.
6. Use `/team reload` after editing the configuration.

This is a server-side mod. Players do not need to install it on their clients.

## Commands

```text
/team help
/team create <name>
/team invite <player>
/team join-req <team>
/team accept [player]
/team decline [player]
/team requests
/team chat
/team lists
/team info
/team modify
/team modify color <color>
/team modify friendlyFire <true|false>
/team members
/team coords <player>
/team rename <name>
/team transfer <player>
/team alias <player> <alias>
/team unalias <player>
/team kick <player>
/team leave
/team disband
/team glow <true|false>
```

The mod replaces the vanilla scoreboard `/team` command root. Vanilla scoreboard commands such as `/team add` and `/team empty` are therefore not included.

## Configuration and integrations

The configuration is created at `config/zyns-better-teams/config.yml` after the first server start. Review the generated comments before changing settings. Some changes may require a restart; `/team reload` reloads supported live settings.

See `integrations/README.md` in the source packages for the optional integration notes.

## Source and test builds

The project has separate source packages and compiled test JARs for the three compatibility targets. The repository's Releases page is the intended public download location. Test binaries are not labelled as stable releases.

- [GitHub releases](https://github.com/ZynAyush/zyns-better-teams/releases)
- [Project guide and compatibility details](https://zynayush.github.io/docs/zyns-better-teams/)
- [Modrinth project page](https://modrinth.com/mod/zyns-better-teams) (pending moderation)

## Reporting an issue

Open a [GitHub issue](https://github.com/ZynAyush/zyns-better-teams/issues/new) and include your Minecraft version, Fabric Loader version, Fabric API version, mod build, relevant logs and steps to reproduce the issue.

## License

See [LICENSE](LICENSE).