# minga

> Sovereign P2P sharing with a content-addressed FUSE mount, in Rust.

`minga` (Quechua: *collective work*) shares content peer-to-peer: multi-bundle packs, content-addressed (BLAKE3) storage, and a FUSE filesystem so shared content mounts as real files. Discovery and transport ride the `card`/`chasqui` networking layer (relay, dcutr, autonat — NAT-traversal included).

## How dependencies work
Front-door repo: only `minga-*` crates here. The `card` identity primitives, shared leaves and UI are git-dependencies of the [`gioser`](https://gitea.gioser.net/sergio/gioser) monorepo (source of truth).

## License
MIT. Part of the [gioser](https://gitea.gioser.net/sergio/gioser) suite.
