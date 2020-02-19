The following are solutions from the REGEX tutorial [regexcrosswords](https://regexcrossword.com/).

### Tutorial

#### (1) the OR symbol

|                 | A&#124;B |
|:---------------:|:--------:|
| <b>A&#124;Z</b> | A        |

#### (2) a range of characters

|              | [ABC] |
|:------------:|:-----:|
| <b>[BDF]</b> | B     |

#### (3) characters NOT to include

|              | [^AB] |
|:------------:|:-----:|
| <b>[ABC]</b> | C     |

#### (4) zero or more

|            | A*  |
|:----------:|:---:|
| <b>A</b>   | A   |
| <b>AB+</b> | A   |

#### (5) zero or one

|                 | A?B? |
|:---------------:|:----:|
| <b>A&#124;C</b> | A    |
| <b>B</b>        | B    |

#### (6) one or more

|                 | A+  |
|:---------------:|:---:|
| <b>A&#124;B</b> | A   |
| <b>A&#124;Z</b> | A   |

#### (7) backreference

|                 | (A)\1 |
|:---------------:|:-----:|
| <b>A&#124;B</b> | A     |
| <b>A&#124;B</b> | A     |

#### (8) specific amount

|                 | A{2,} |
|:---------------:|:-----:|
| <b>A{1}</b>     | A     |
| <b>B&#124;A</b> | A     |

#### (9) space

|           | A&#124;\s |
|:---------:|:---------:|
| <b>\s</b> | \s        |

Hint: 
- Must use normal " " character instead of `\s`.

### Beginner

#### (1) beatles

|                           | [^SPEAK]+ | EP&#124;IP&#124;EF |
|:-------------------------:|:---------:|:------------------:|
| <b>HE&#124;LL&#124;O+</b> | H         | E                  |
| <b>[PLEASE]+</b>          | L         | P                  |

Hint: 
- `[^SPEAK]` means any character <b>NOT</b> present in list.


#### (2) naughty

|                             | (A&#124;B&#124;C)\1 | (AB&#124;OE&#124;SK) |
|:---------------------------:|:-------------------:|:--------------------:|
| <b>.&#42;M?O.&#42;</b>      | B                   | O                    |
| <b>(AN&#124;FE&#124;BE)</b> | B                   | E                    |

Hint: 

- In the pattern `.*M?O.*`, an `O` <b>must</b> be present for a match to happen.

- `\1` makes back reference to match same text of the first group again.

#### (3) ghost

|                 | [COBRA]+ | (AB&#124;O&#124;OR)+ |
|:---------------:|:--------:|:--------------------:|
| <b>(.)+\1</b>   | O        | O                    |
| <b>[^ABRC]+</b> | O        | O                    |

#### (4) symbolism

|             | .?.+ | .+  |
|:-----------:|:----:|:---:|
| <b>[*]+</b> | *    | *   |
| <b>/+</b>   | /    | /   |

Hint:

- `[*]` Matches the `*` character literally.