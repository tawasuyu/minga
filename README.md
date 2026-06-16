# minga

> Sovereign P2P sharing with a content-addressed FUSE mount, in Rust.

`minga` (Quechua: *collective work*) shares content peer-to-peer: multi-bundle packs, content-addressed (BLAKE3) storage, and a FUSE filesystem so shared content mounts as real files. Discovery and transport ride the `card`/`chasqui` networking layer (relay, dcutr, autonat — NAT-traversal included).

<p align="center">
  <img src="docs/minga_showreel.gif" alt="minga showreel — the repo explorer: AST nodes in the content-addressed store, Ed25519 attestations vouching for them, and Merkle-Search-Tree keys" width="900">
  <br>
  <sub>the repo explorer — content-addressed AST nodes, Ed25519 attestations &amp; Merkle-Search-Tree keys</sub>
</p>

## How dependencies work
Front-door repo: only `minga-*` crates here. The `card` identity primitives, shared leaves and UI are git-dependencies of the [`tawasuyu`](https://github.com/tawasuyu/tawasuyu) monorepo (source of truth).

## License
MIT. Part of the [tawasuyu](https://github.com/tawasuyu/tawasuyu) suite.
