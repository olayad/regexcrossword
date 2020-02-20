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

#### (5) airstrip one

|                           | \d[2480] | 56&#124;94&#124;73 |
|:-------------------------:|:--------:|:------------------:|
| <b>18&#124;19&#124;20</b> | 1        | 9                  |
| <b>[6789]\d</b>           | 8        | 4                  |

### Intermediate

#### (1) always remember

|                              | UB&#124;IE&#124;AW | [TUBE]* | [BORF]. |
|:----------------------------:|:------------------:|:-------:|:-------:|
| <b>[NOTAD]*</b>              | A                  | T       | O       |
| <b>WEL&#124;BAL&#124;EAR</b> | W                  | E       | L       |

#### (2) johnny

|                             | [BQW]&#40;PR&#124;LE) | [RANK]+ |
|:---------------------------:|:---------------------:|:-------:|
| <b>[AWE]+</b>               | W                     | A       |
| <b>[ALP]+K</b>              | L                     | K       |
| <b>(PR&#124;ER&#124;EP)</b> | E                     | R       |

#### (3) earth

|                              | .(.)\1 | .*[WAY]+ | [RAM].[OH] |
|:----------------------------:|:------:|:--------:|:----------:|
| <b>CAT&#124;FOR&#124;FAT</b> | F      | O        | R          |
| <b>RY&#124;TY\-</b>          | T      | Y        | -          |
| <b>[TOWEL]*</b>              | T      | W        | O          |

Hint: 

- In `.(.)\1`, the `\1` references the first group captured. In this case, `.(.)\1` means the letter captured is repeated.


#### (4) encyclopedia

|                      | [JUNDT]* | APA&#124;OPI&#124;OLK | (NA&#124;FE&#124;HE)[CV] |
|:--------------------:|:--------:|:---------------------:|:------------------------:|
| <b>[DEF][MNO]*</b>   | D        | O                     | N                        |
| <b>[^DJNU]P[ABC]</b> | T        | P                     | A                        |
| <b>[ICAN]*</b>       | N        | I                     | C                        |

#### (5) technology

|                 | [^NRU]&#40;NO&#124;ON) | (D&#124;FU&#124;UF)+ | (FO&#124;A&#124;R)* | (N&#124;A)* |
|:---------------:|:----------------------:|:--------------------:|:-------------------:|:-----------:|
| <b>[RUNT]*</b>  | T                      | U                    | R                   | N           |
| <b>O.*[HAT]</b> | O                      | F                    | F                   | A           |
| <b>(.)*DO\1</b> | N                      | D                    | O                   | N           |

### Experienced

#### (1) royal dinner

|                                  | (FI&#124;A)+ | (YE&#124;OT)K | (.)[IF]+ | [NODE]+ | (FY&#124;F&#124;RG)+ |
|:--------------------------------:|:------------:|:-------------:|:--------:|:-------:|:--------------------:|
| <b>(Y&#124;F)(.)\2[DAF]\1</b>    | F            | O             | O        | D       | F                    |
| <b>(U&#124;O&#124;I)*T[FRO]+</b> | I            | T             | F        | O       | R                    |
| <b>[KANE]&#42;[GIN]*</b>         | A            | K             | I        | N       | G                    |

#### (2) regular workout

|                              |[ARK]&#42;O.&#42;|(.).&#42;\1N\1|(SOD&#124;DO&#124;GE)&#42;|[FAXUS]&#42;|[LOPITY]&#42;|
|:----------------------------:|:---------------:|:------------:|:------------------------:|:----------:|:-----------:|
| <b>[UGLER]*</b>              | R               | E            | G                        | U          | L           |
| <b>[CAST]&#42;REX[PEA]*</b>  | A               | R            | E                        | X          | P           |
| <b>[SIRES]*</b>              | R               | E            | S                        | S          | I           |
| <b>(L&#124;OFT&#124;ON)*</b> | O               | N            | O                        | F          | T           |
| <b>H&#42;(AY&#124;ED)*</b>   | H               | E            | D                        | A          | Y           |

#### (3) We apologise for the inconvenience

|                              |[ABC]*(.)\1(ME&#124;UO) | (.)T\*E*\1 | [HAS]*(SN&#124;PA)| (WE&#124;GA&#124;AL)T*O+ | (EG&#124;BEEE)[WIQ]* |
|:----------------------------:|:----------------------:|:----------:|:-----------------:|:------------------------:|:--------------------:|
| <b>[QA].[WEST]*</b>          | A                      | N          | S                 | W                        | E                    |
| <b>(HE&#124;RT&#124;TK)*.</b>| R                      | T          | H                 | E                        | G                    |
| <b>(RE&#124;QR)[QUART]*</b>  | R                      | E          | A                 | T                        | Q                    |
| <b>[EUW]*S[RITE]*</b>        | U                      | E          | S                 | T                        | I                    |
| <b>(.)(.)\2\1[WE]</b>        | O                      | N          | N                 | O                        | W                    |
