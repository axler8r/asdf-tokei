# asdf-tokei

[tokei](https://github.com/XAMPPRocky/tokei) plugin for the [asdf version manager](https://asdf-vm.com).

This plugin builds tokei from source using Cargo.

## Contents

- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

## Dependencies

**Required:**
- `bash`, `curl`, `tar`: generic POSIX utilities
- `git`: for listing versions
- `cargo`: Rust toolchain for building from source

**Install Rust/Cargo:**
```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Install

Plugin:

```shell
asdf plugin add tokei https://github.com/AxlER8R/asdf-tokei.git
```

tokei:

```shell
# Show all installable versions
asdf list-all tokei

# Install specific version (including v13.0.0)
asdf install tokei 13.0.0

# Install latest
asdf install tokei latest

# Set a version globally (on your ~/.tool-versions file)
asdf global tokei latest

# Now tokei commands are available
tokei --version
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to install & manage versions.

## Contributing

Contributions of any kind welcome! See the [contributing guide](CONTRIBUTE.md).

## License

See [LICENSE](LICENSE)
