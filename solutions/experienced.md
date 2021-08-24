### Royal Dinner

|                       | (FI\|A)+ | (YE\|OT)K | (.)[IF]+ | [NODE]+ | (FY\|F\|RG)+ |
|:---------------------:|:--------:|:---------:|:--------:|:-------:|:------------:|
| <b>(Y\|F)(.)\2[DAF]\1 | F        | O         | O        | D       | F            |
| <b>(U\|O\|I)\*T[FRO]+ | I        | T         | F        | O       | R            |
| <b>[KANE]\*[GIN]\*    | A        | K         | I        | N       | G            |

Explanation:
* (FI|A)+ equals 1 or more of group of `FI` or `A`
* (YE|OT)K equals a group of `YE` or `OT` followed by `K'
* (.)[IF]+ equals a group of `*` followed by 1 or more of a character from `IF`
* [NODE]+ equals 1 or more or a character from `NODE`
* (FY|F|RG)+ equals 1 or more of a group of `FY` or `F` or `RG`

* (Y|F)(.)\2[DAF]\1
* (U|O|I)*T[FRO]+ equals 0 or more of a group of `U` or `O` or `I` followed by a `T` followed by 1 or more of a character from `FRO`
* [KANE]\*[GIN]\* equals 0 or more of a character from `KANE` followed by 0 or more of a character from `GIN`

### Regular Workout

|                         | [ARK]\*O.\* | (.).\*\1N\1 | (SOD\|DO\|GE)\* | [FAXUS]\* | [LOPITY]\* |
|:-----------------------:|:-----------:|:-----------:|:---------------:|:---------:|:----------:|
| <b>[UGLER]\*            | R           | E           | G               | U         | L          |
| <b>[CAST]\*REX[PEA]\*   | A           | R           | E               | X         | P          |
| <b>[SIRES]\*            | R           | E           | S               | S         | I          |
| <b>(L\|OFT\|ON)\*       | O           | N           | O               | F         | T          |
| <b>H\*(AY|ED)\*         | H           | E           | D               | A         | Y          |

Explanation:
* [ARK]*O.* equals a character from `BQW` followed by a group of `PR` or `LE`
* (.).*\1N\1 equals 1 or more of a character from `RANK`
* (SOD|DO|GE)* equals 1 or more of a character from `AWE`
* [FAXUS]* equals 1 or more of a character from `ALP` followed by a `K`
* [LOPITY]* equals `PR` or `ER` or `EP`

* [UGLER]*
* [CAST]*REX[PEA]*
* [SIRES]*
* (L|OFT|ON)*
* H*(AY|ED)*

### Earth

|                | .(.)\1 | .*[WAY]+ | [RAM].[OH] |
|:--------------:|:------:|:--------:|:----------:|
| <b>CAT\|FOR\|FAT | F      | O        | R
| <b>RY\|TY\-     | T      | Y        | -
| <b>[TOWEL]*    | T      | W        | O

Explanation:
* .(.)\1 equals 1 or more of any character except newline followed by a backreference to a group of any character except newline
* .*[WAY]+ equals 1 or more of any character except newline followed by 1 or more of a chracter from `WAY`a group of `AB` or `O` or `OR`
* [RAM].[OH] equals a character from `RAM` followed by any character except newline followed by a character from `OH`
* CAT|FOR|FAT equals `CAT` OR `FOR` or `FAT`
* RY|TY\- equals `RY` or `TY` followed by `-`
* [TOWEL]* equals 0 or more of a character from `TOWEL`

### Encyclopedia

|                  | [JUNDT]* | APA\|OPI\|OLK | (NA\|FE\|HE)[CV] |
|:----------------:|:--------:|:-------------:|:----------------:|
| <b>[DEF][MNO]*   | D        | O             | N
| <b>[^DJNU]P[ABC] | T        | P             | A
| <b>[ICAN]*       | N        | I             | C

Explanation:
* [JUNDT]* equals 1 or more of a character from `JUNDT`
* APA|OPI|OLK equals `APA` or `OPI` or `OLK`
* (NA|FE|HE)[CV] equals `NA` or `FE` or `HE` followed by a character from `CV`
* [DEF][MNO]* equals a character from `DEF` followed by 0 or more of a character from `MNO`
* [^DJNU]P[ABC] equals a character not from `DJNU` followed by `P` followed by a character from `ABC`
* [ICAN]* equals 1 or more of a character from `ICAN`

### Technology

|             | \[^NRU\](NO\|ON) | (D\|FU\|UF)+ | (FO\|A\|R)* | (N\|A)* |
|:-----------:|:--------------:|:------------:|:-----------:|:-------:|
| <b>[RUNT]*  | T              | U            | R           | N       |
| <b>O.*[HAT] | O              | F            | F           | A       |
| <b>(.)*DO\1 | N              | D            | O           | N       |

Explanation:
* \[^NRU]\(NO|ON) equals a character not from `NRU` followed by group of `NO` or `ON`
* (D|FU|UF)+ equals 1 or more of group of `D` or `FU` or `UF`
* (FO|A|R)* equals 0 or more of group of `FO` or `A` or `R`
* (N|A)* equals 0 or more of group of `N` or `A`

* [RUNT]* equals 1 or more of a character from `RUNT`
* O.*[HAT] equals `O` followed by 1 or more of any character except newline followed by a character from `HAT`
* (.)*DO\1 equals 0 or more of group of `*` followed by`DO` followed by a backreference to 1st group, `*`
  
### Hamlet

|             | [RUTH]*(OE|EO)[RB]* | (BG|ON|KK)+[RIF]+ | (MN|BO|FI)[EU]{2,} | (KT|AL|ET)+G | [OH](PR|AX|TR)+ |
|:-----------:|:--------------:|:------------:|:-----------:|:-------:|
| <b>[IT](O)*(BE|AD)*\1  | T              | O            | B           | E       | O |
| <b>[NORMAL]+T{2} | R              | N            | O           | T       | T |
| <b>.*(XA|BE).* | O              | B            | E           | A       | R|
| <b>(EG|UL){2}[ALF]* | E              | G            | U           | L    | A |
| <b>[REQ]*(G|P)(.)+ | R              | R            | E           | G       |X|

Explanation:
* [RUTH]*(OE|EO)[RB]* equals a character not from `NRU` followed by group of `NO` or `ON`
* (BG|ON|KK)+[RIF]+ equals 1 or more of group of `D` or `FU` or `UF`
* (MN|BO|FI)[EU]{2,} equals 0 or more of group of `FO` or `A` or `R`
* (KT|AL|ET)+G equals 0 or more of group of `N` or `A`
* [OH](PR|AX|TR)+
  
* [IT](O)*(BE|AD)*\1 equals 1 or more of a character from `RUNT`
* [NORMAL]+T{2} equals `O` followed by 1 or more of any character except newline followed by a character from `HAT`
* .*(XA|BE).* equals 0 or more of group of `*` followed by`DO` followed by a backreference to 1st group, `*`
* (EG|UL){2}[ALF]* equals either EG or UL 2 times followed by 0 or more of the optional group of A, L, F
* [REQ]*(G|P)(.)+ equals 0 or more of the optional group R, E, Q
