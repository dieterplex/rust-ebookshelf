# The Rust eBookshelf

[![Build Status](https://travis-ci.org/rams3s/rust-ebookshelf.svg?branch=master)](https://travis-ci.org/rams3s/rust-ebookshelf)

This [project](https://rams3s.github.io/rust-ebookshelf) aims at providing nightly builds of all official rust mdbooks in epub format.
It is born out of the difficulty I encountered when starting my rust apprenticeship to find recent ebook versions of the official documentation.

If you encounter any issue, have any suggestion or would like to improve this site and/or its content, please go to <https://github.com/rams3s/rust-ebookshelf/> and file an issue or create a pull request.

If you find this useful, please let me know so by saying hi on twitter [@Rams3s](https://twitter.com/Rams3s).

Happy coding.


## Building books

Install mdbookshelf from [dieterplex/mdbookshelf](https://github.com/dieterplex/mdbookshelf)

```
cargo install --git https://github.com/dieterplex/mdbookshelf
```

### Known issue

- Many books still contain fatal errors checking with `epubcheck` tool. Some readers may not work as expected.
- TRPL won't be able to build correct book content since `rustdoc_include` is not supported by [mdbook-epub standalone mode](https://github.com/Michael-F-Bryan/mdbook-epub/issues/30). Manually use `mdbook build` after the line `[output.epub]` appended to `book.toml`.



