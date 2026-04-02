# prunus-config

Configuration files for prunus — capture profiles and server settings.

Companion repository to the main [prunus](../prunus) project.

## Structure

```
cfg/
  profiles/          # Capture profile definitions (## Capture / ## Skip sections)
```

## Usage

Profiles are enabled per-tree via symlinks. Use the MCP tools `enable_profile` / `disable_profile` from within a client session, or create symlinks manually:

```sh
ln -s /path/to/prunus-config/cfg/profiles/software-architect.md /path/to/grove/tree/.profiles/software-architect.md
```

The server combines all enabled profiles' `## Capture` and `## Skip` sections and injects them into the LLM extraction prompt.
