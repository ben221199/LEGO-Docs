# SRF - <ins>S</ins>t<ins>r</ins>ing <ins>F</ins>ile

This file is used in:
 - LEGO Racers

## Header

| Offset (from start file) | Length (in bytes) | Type | Description |
| - | - | - | - |
| 0x00 | 2 | INT16LE | Amount of strings in file |
| 0x02 | 2 | INT16LE | Amount of characters in file |

> Note: Characters are two bytes long. The NULL characters are also counted.

## Offset table

| Offset (from start file) | Length (in bytes) | Type | Description |
| - | - | - | - |
| 0x04 | 2 | INT16LE | Offset of string #1 |
| 0x06 | 2 | INT16LE | Offset of string #2 |
| 0x08 | 2 | INT16LE | Offset of string #3 |
| ... | ... | ... | ... |

etc.

> Note: The offset in the offset table starts counting from the end of the offset table, so the first string has offset 0x00. Seen from the start of the file, it is offset 0x04.

## Strings

| Offset (from start file) | Length (in bytes) | Type | Description |
| - | - | - | - |
| offset #1 + 0x04 | variable | String | String #1 |
| offset #2 + 0x04 | variable | String | String #2 |
| offset #3 + 0x04 | variable | String | String #3 |
| ... | ... | ... | ... |

etc.

> Note: All strings end with a NULL-character. The string can also contain line feeds (0x0A).
