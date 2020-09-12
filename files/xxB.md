# <sub><i>xx</i></sub>B - ... <ins>B</ins>inary

This file is used in:
 - LEGO Racers
 
 ## Types
 
 | Byte | Description |
| - | - |
| 0x02 | String (NULL-terminated) |
| 0x03 | Float (32 bit) |
| 0x04 | Int (32 bit) |
| 0x05 | Dictionary start (`{`) |
| 0x06 | Dictionary end (`}`) |
| 0x07 | List start (`[`) |
| 0x08 | List end (`]`) |
| 0x0B | <ul style="margin:0px;"><li>Signed Byte (8 bits)</li><li>Fraction (8 bits)</li></ul> |
| 0x0C | Unsigned Byte (8 bits) |
| 0x0D | <ul style="margin:0px;"><li>Signed Short (16 bits)</li><li>Fraction (16 bits)</li></ul> |
| 0x0E | Unsigned Short (16 bits) |
| 0x14 | Array |
| 0x16 | Struct |

### String

A string that ends in a 0x00.

### Float

A 32-bit float.

### Int

A 32-bit integer.

### Dictionary

A dictionary of key-value paired items which can be of different types. Starts with `0x05` and ends `0x06`.

### List

A list of items which can be of different types. Starts with `0x07` and ends `0x08`.

### Byte

Signed, Unsigned or fraction.

### Short

Signed, Unsigned or fraction.

### Array

An array.

 - Length (short)
 - Type (Byte)
 - Items

### Struct

A struct.

 - Id (Byte, type)
 - Length (Byte)
