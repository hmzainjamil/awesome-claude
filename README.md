# Awesome Claude

A small public repository for Claude-related projects and resources. The package metadata identifies the project as an awesome list and names [Alvin Unreal](https://github.com/alvinunreal) as author; preserve that attribution. The metadata points to [alvinunreal/awesome-claude](https://github.com/alvinunreal/awesome-claude) as the upstream repository.

## At a glance

| Field | Details |
|---|---|
| Repository package | `awesome-claude` |
| Package version | `1.0.0` |
| Upstream license | CC0-1.0; see [LICENSE](./LICENSE) |
| Included subproject | [Claude VSCode Theme](./claude-vscode-theme/README.md), separately licensed MIT |
| Quality checks | `npm run lint`, `npm test`, `npm run check-links` |

## Current contents

The tracked repository includes a Claude VS Code theme project with four theme variants. The root README currently has no resource catalog entries, despite the package being described as an awesome list. I’m recording that gap instead of inventing entries. Add resources only with verified project links, concise descriptions, and attribution.

The theme is a distinct subproject with its own package metadata, build scripts, and MIT license. See its [README](./claude-vscode-theme/README.md) for installation, variants, screenshots, and build details.

## Contributing

Use the repository's [contribution guidelines](./contributing.md). Check that links work and project status and licensing are described accurately. Resource inclusion does not imply endorsement, security review, or compatibility.

## Validation

The root package defines:

- `npm run lint`: run `awesome-lint` on this README.
- `npm test`: runs the lint script.
- `npm run check-links`: checks README links with the checked-in link-check configuration.

These scripts were not run for this documentation update.

## Scope and limitations

This repository is a collection and includes an independently packaged editor theme. It does not provide a Claude API client, agent runtime, tool router, fallback model system, or repository-wide security controls. External resources can change; check their current documentation and licenses before use.

The theme package has its own MIT license. The root package metadata declares CC0-1.0. Review the applicable license file before reusing files from either part of the repository.
