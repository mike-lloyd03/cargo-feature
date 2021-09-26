# cargo-feature

![preview](https://github.com/Riey/cargo-feature/blob/master/preview.png)

## Install

### Cargo

`cargo install cargo-feature`

### NixOS

`nix-env -iA nixos.cargo-feature`

### AUR

`paru -S cargo-feature`

## Usage

```
# add serde_derive feature to build-dependency of serde
cargo feature -t build serde +serde_derive

# disable default-features
cargo feature serde ^default

# same as above but more explict
cargo feature serde --disable-default-features

# enable default-features
cargo feature serde default

# same as above but more explict
cargo feature serde --enable-default-features

# add HtmlDivElement feature to dependency of web_sys 
cargo feature web_sys +HtmlDivElement

# you can skip typing +
cargo feature web_sys HtmlDivElement

# same as above but remove
cargo feature web_sys ^HtmlDivElement
```
