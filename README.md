<!--
[![Crate](https://img.shields.io/crates/v/quircs.svg?style=flat-square)](https://crates.io/crates/sqr)
[![Downloads](https://img.shields.io/crates/d/quircs.svg?style=flat-square)](https://crates.io/crates/sqr)
[![Docs](https://img.shields.io/badge/docs-latest-blue.svg?style=flat-square)](https://docs.rs/sqr)-->
[![Dependencies](https://deps.rs/repo/github/pepa65/sqr/status.svg)](https://deps.rs/repo/github/pepa65/sqr)
[![CI](https://github.com/pepa65/sqr/workflows/CI/badge.svg)](https://github.com/pepa65/sqr/actions)
[![License](https://img.shields.io/github/license/pepa65/sqr)](https://github.com/pepa65/sqr/blob/main/LICENSE)

# sqr 0.11.0
**Scan QR with Quircs**

* After: <https://github.com/dignifiedquire/quircs> which was ported from <https://github.com/dlbeer/quirc>
* Repo: <https://github.com/pepa65/sqr>

## Install
### Download and install static single-binary
```
wget https://github.com/pepa65/sqr/releases/download/0.11.0/sqr
sudo mv sqr /usr/local/bin
sudo chown root:root /usr/local/bin/sqr
sudo chmod +x /usr/local/bin/sqr
```

## Install with cargo
If not installed yet, install a **Rust toolchain**, see <https://www.rust-lang.org/tools/install>

### Static build for Linux (avoiding GLIBC incompatibilities)
```
git clone https://github.com/pepa65/sqr
cd sqr
rustup target add x86_64-unknown-linux-musl
cargo rel  # Alias defined in .cargo/config.toml
```

The binary will be at `target/x86_64-unknown-linux-musl/release/sqr`

## Usage
```
sqr 0.11.0
Usage:  sqr [-h|--help] | [-v|--verbose] <image>...
```
