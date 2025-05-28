# DaletPack specification for Dalet v1.0-preview

DaletPack is an binary data format for Dalet, that is used for minimizing the size of transmitted data.

- DaletPack is serialized with [serde](https://serde.rs/) and [bitcode v0.6.6](https://docs.rs/bitcode/0.6.6/bitcode/) Page struct from [dalet-rs types](https://github.com/TempoWorks/dalet-rs/blob/main/src/types.rs)
- All apps that supports Dalet must use this format when transmitting data between hosts.
- All data must be compressed with [zstd](https://datatracker.ietf.org/doc/html/rfc8878).
- Mime type: `application/dalet-pack`
