### Always remember

|                  | UB\|IE\|AW | [TUBE]* | [BORF]. |
|:----------------:|:----------:|:-------:|:-------:|
| <b>[NOTAD]*      | A          | T       | O       |
| <b>WEL\|BAL\|EAR | W          | E       | L       |

Explaination: 
* UB|IE|AW equals  `UB` or `IE` or `AW`
* [TUBE]* equals 0 or more of a character from `TUBE`
* [BORF]. equals a character from `BORF` followed by any character except newline
* [NOTAD]* equals 0 or more of a character from `NOTAD`
* WEL|BAL|EAR equals `WEL` or `BAL` or `EAR``  

### Johnny

|               | [BQW](PR\|LE) | [RANK]+ |
|:-------------:|:-------------:|:-------:|
| <b>[AWE]+     | W             | A       |
| <b>[ALP]+K    | L             | K       |
| <b>(PR\|ER\|EP) | E             | R       |

Explaination: 
* [BQW](PR\|LE) equals a character from `BQW` followed by a group of `PR` or `LE`
* [RANK]+ equals 1 or more of a character from `RANK`
* [AWE]+ equals 1 or more of a character from `AWE`
* [ALP]+K equals 1 or more of a character from `ALP` followed by a `K`
* (PR|ER|EP) equals `PR` or `ER` or `EP` 

### Earth

|                | .(.)\1 | .*[WAY]+ | [RAM].[OH] |
|:--------------:|:------:|:--------:|:----------:|
| <b>CAT\|FOR\|FAT | F      | O        | R
| <b>RY\|TY\-     | T      | Y        | -
| <b>[TOWEL]*    | T      | W        | O

Explaination: 
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

Explaination: 
* [JUNDT]* equals 1 or more of a character from `JUNDT`
* APA|OPI|OLK equals `APA` or `OPI` or `OLK`
* (NA|FE|HE)[CV] equals `NA` or `FE` or `HE` followed by a character from `CV`
* [DEF][MNO]* equals a character from `DEF` followed by 0 or more of a character from `MNO`
* [^DJNU]P[ABC] equals a character not from `DJNU` followed by `P` followed by a character from `ABC`
* [ICAN]* equals 1 or more of a character from `ICAN`

### Technology

|             | [^NRU](NO\|ON) | (D\|FU\|UF)+ | (FO\|A\|R)* | (N\|A)* |
|:-----------:|:--------------:|:------------:|:-----------:|:-------:|
| <b>[RUNT]*  | T              | U            | R           | N       |
| <b>O.*[HAT] | O              | F            | F           | A       |
| <b>(.)*DO\1 | N              | D            | O           | N       |

Explaination: 

* [^NRU](NO|ON) equals a character not from `NRU` followed by group of `NO` or `ON`
* (D|FU|UF)+ equals 1 or more of group of `D` or `FU` or `UF`
* (FO|A|R)* equals 0 or more of group of `FO` or `A` or `R`
* (N|A)* equals 0 or more of group of `N` or `A`

* [RUNT]* equals 1 or more of a character from `RUNT`
* O.*[HAT] equals `O` followed by 1 or more of any character except newline followed by a character from `HAT`
* (.)*DO\1 equals 0 or more of group of `*` followed `DO` followed by a backreference to 1st group, `*`