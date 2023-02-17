# The Rust eBookshelf

![GH-Pages Build Status](https://github.com/dieterplex/rust-ebookshelf/actions/workflows/gh-pages.yml/badge.svg)

This [project](https://dieterplex.github.io/rust-ebookshelf) aims at providing nightly builds of all official rust mdbooks in epub format.
It is born out of the difficulty I encountered when starting my rust apprenticeship to find recent ebook versions of the official documentation.

If you encounter any issue, have any suggestion or would like to improve this site and/or its content, please go to <https://github.com/dieterplex/rust-ebookshelf/> and file an issue or create a pull request.

If you find this useful, please let me know so by saying hi on twitter [@Rams3s](https://twitter.com/Rams3s).

Happy coding.

## Building books

Install mdbookshelf from [dieterplex/mdbookshelf](https://github.com/dieterplex/mdbookshelf)

```console
cargo install --git https://github.com/dieterplex/mdbookshelf
```

### Known issue

- Many books still contain fatal errors by checking with `epubcheck` tool. Some readers may not work as expected.
