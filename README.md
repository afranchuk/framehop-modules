# `framehop-object`

This crate provides an implementation of `framehop::ModuleSectionInfo` for the `object` crate, to
make using the two crates together easy. It attempts to support different combinations of `framehop`
and `object` versions for maximum flexibility. If you encounter a breaking version combination
please submit an issue!

## Version Compatibility

| Crate Version | Framehop Version(s) | Object Version(s) |
| ------------- | ------------------- | ----------------- |
| 0.1.0         | >= 0.9              | >=0.30,<0.35      |
| 0.2.0         | >= 0.9              | >=0.35            |

## Usage

The crate exposes a `ObjectSectionInfo` wrapper. When created with a type implementing
`object::read::Object`, it will implement `framehop::ModuleSectionInfo` using that type.
