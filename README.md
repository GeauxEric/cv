# lambda-twist

[![Discord][dci]][dcl] [![Crates.io][ci]][cl] ![MIT/Apache][li] [![docs.rs][di]][dl] ![LoC][lo] ![Tests][btl] ![Lints][bll] ![no_std][bnl]

[ci]: https://img.shields.io/crates/v/lambda-twist.svg
[cl]: https://crates.io/crates/lambda-twist/

[li]: https://img.shields.io/crates/l/specs.svg?maxAge=2592000

[di]: https://docs.rs/lambda-twist/badge.svg
[dl]: https://docs.rs/lambda-twist/

[lo]: https://tokei.rs/b1/github/rust-cv/lambda-twist?category=code

[dci]: https://img.shields.io/discord/550706294311485440.svg?logo=discord&colorB=7289DA
[dcl]: https://discord.gg/d32jaam

[btl]: https://github.com/rust-cv/lambda-twist/workflows/unit%20tests/badge.svg
[bll]: https://github.com/rust-cv/lambda-twist/workflows/lints/badge.svg
[bnl]: https://github.com/rust-cv/lambda-twist/workflows/no-std/badge.svg

Relative camera pose from three 3d to 2d correspondences

To see an example of usage, see `tests/consensus.rs`.

This was derived from <https://github.com/rust-cv/p3p/>. It was rewritten to utilize Rust CV abstractions.

Implementation based on
"Lambda Twist: An Accurate Fast Robust Perspective Three Point (P3P) Solver"
Persson, M. and Nordberg, K. ECCV 2018.

Reference implementation available on the [author github repository][lambda-twist-github].

[lambda-twist-github]: https://github.com/midjji/lambdatwist-p3p

## Documentation

To build the documentation with math formatted by katex:

```bash
RUSTDOCFLAGS="--html-in-header katex-header.html" cargo doc --no-deps
```

## License

This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.
If a copy of the MPL was not distributed with this file,
You can obtain one at <http://mozilla.org/MPL/2.0/>.

This rewrite is based on the adaptation of the original code (GPL-3.0)
into [OpenMVG, published under MPL-2.0 with the original author agreement][p3p-openmvg].

[p3p-openmvg]: https://github.com/openMVG/openMVG/pull/1500
