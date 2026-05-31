# pleme-verification-matrix

The farm's first TEST-generation primitive: a dependency-free declarative-macro crate exposing verification_matrix! (one aggregate #[test] over a typed const ROWS: &[Row] table, aggregating every failure before assert) + matrix_covers_all! (a #[test] build-gate asserting ROWS.len() == an enum's variantcount COUNT). Realizes the CLOSED-LOOP MASS-SYNTHESIS verification-matrix-as-forcing-function rule as a consumable; composes with pleme-variantcount-derive.

[![Build](https://github.com/pleme-io/pleme-verification-matrix/actions/workflows/auto-release.yml/badge.svg)](#)
[![crates.io](https://img.shields.io/crates/v/pleme-verification-matrix.svg)](https://crates.io/crates/pleme-verification-matrix)

## Install

```toml
[dependencies]
pleme-verification-matrix = "*"
```

## Generation

This crate is mechanically emitted by [`tatara-rust-ast`](https://github.com/pleme-io/tatara-rust-ast). The author surface is a typed `(defmacro …)` Spec — the proc-macro implementation, tests, Nix flake, caixa wrapper, and CI workflow are all generated. See the catalog at `catalog.json` in the parent registry.
