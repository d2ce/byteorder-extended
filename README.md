# byteorder-extended

This crate, based on [scalexm/holomorph](https://github.com/scalexm/holomorph/blob/master/protocol/src/io.rs), provides an extension of functions to read/write streams.

## Installation

```toml
[dependencies]
byteorder_extended = { git = "https://github.com/d2ce/byteorder-extended" }
```

## Example

```rust
extern crate byteorder_extended;

use std::io::Cursor;

use byteorder_extended::ReadExt;

/// ...

let mut buffer = Cursor::new(vec![0; 4]);
let value = buffer.read_i32()?;

/// ...

```

## License

`byteorder-extended` is distributed under the terms the MIT license.

Substantial portions of the code might come from `holomorph` crate. 
`holomorph` is distributed under the terms of the MIT license. Make 
sure to include it on the end  product.