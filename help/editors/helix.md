1. Install dalet_lsp `cargo install dalet_lsp`
2. Add this to languages.toml:

```toml
[[language]]
name = "dalet"
language-servers = ["dalet-lsp"]
auto-format = true
scope = "source.dalet"
file-types = ["dm", "dss"]

[language-server.DaletMark-lsp]
command = "dalet_lsp"

[[grammar]]
name = "Dalet"

[grammar.source]
git = "https://github.com/TxtDot/tree-sitter-dalet"
rev = "HEAD"
```
