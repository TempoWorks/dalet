1. Install DaletMark_lsp `cargo install DaletMark_lsp`
2. Add this to languages.toml:

```toml
[[language]]
name = "DaletMark"
language-servers = ["DaletMark-lsp"]
auto-format = true
scope = "source.DaletMark"
file-types = ["dlth"]

[language-server.DaletMark-lsp]
command = "DaletMark_lsp"

[[grammar]]
name = "DaletMark"

[grammar.source]
git = "https://github.com/TxtDot/tree-sitter-DaletMark"
rev = "HEAD"
```
