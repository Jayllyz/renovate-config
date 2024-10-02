# Renovate Configuration

This repository uses [Renovate](https://docs.renovatebot.com/) for automated dependency updates.

## Main Features

1. **Timezone and Schedule**: Set to Europe/Paris, running before 10am on Mondays.
2. **Extended Configurations**: 
   - Uses recommended config
   - Custom manager for Biome versions (pin biome deps)
   - Groups all non-major updates
   - Uses semantic commit type "chore"
3. **Automerge**: Enabled for non-major updates.
4. **Lock File Maintenance**: Runs monthly with automerge enabled.
5. **Dependency Dashboard**: Enabled for better visibility.
6. **Post Update Actions**: Runs `pnpm dedupe` after updates.
7. **Custom Managers**: Includes a custom regex manager for Rust toolchain updates.
8. **Package Rules**: 
   - Groups GitHub Actions updates
   - Custom schedule for Rust toolchain updates

## Usage

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>Jayllyz/renovate-config"]
}
```

For more detailed information on Renovate configuration options, please refer to the [Renovate documentation](https://docs.renovatebot.com/).
