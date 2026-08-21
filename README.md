# osvbng Plugin Generator (retired)

This template is retired. osvbng Go plugins are in-tree: they are
compiled into osvbngd through blank imports, there is no shared-object
loading, and a plugin lands as a pull request under `plugins/community/`
in the main repo. The living template is the `hello` plugin there,
which every build compiles, and the guide is
`docs/architecture/PLUGINS.md`.

This generator targets packages that were removed from osvbng during
2026 (`pkg/cli`, `cmd/osvbngcli/commands`, `pkg/state`,
`pkg/state/paths`) and no longer produces code that compiles. The
decision and its reasons are recorded in the osvbng-context repo,
ADR 0012.

- https://github.com/veesix-networks/osvbng/tree/main/plugins/community/hello
- https://github.com/veesix-networks/osvbng/blob/main/docs/architecture/PLUGINS.md
- https://github.com/veesix-networks/osvbng-context/blob/main/decisions/0012-go-plugins-in-tree-no-external-sdk.md
