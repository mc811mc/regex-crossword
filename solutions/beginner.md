### Beatles

|                  | [^SPEAK]+ | EP\|IP\|EF |
|:----------------:|:---------:|:-------: |
| <b>HE\|LL\|O+  | H         | E        |
| <b>[PLEASE]+ | L         | P        |

Explaination: 
* [^SPEAK]+ equals 1 or more of a character not from `SPEAK`
* EP\|IP\|EF equals `EP` or `IP` or `EF`
* HE\|LL\|O+ equals `HE` or `LL` or 1 or more of `O`
* [PLEASE]+ equals 1 or more of a character from `PLEASE`  

### Naughty

|                   | (A\|B\|C)\1 | (AB\|OE\|SK) |
|:-----------------:|:---------:|:----------:|
| <b>.\*M?O.\*  | B         | O          |
| <b>(AN|FE|BE) | B         | E          |

Explaination: 
* (A|B|C)\1 equals backreference to group `A|B|C` where group is `A` or `B` or `C`
* (AB|OE|SK) equals a group of `AB` or `OE` or `SK`
* .\*M?O.\* equals 0 or more of any character except newline followed by 0 or 1 `M` followed by a `O` followed by 0 or more of any character except newline
* (AN|FE|BE) equals a group of `AN` or `FE` or `BE`  

### Ghost

|                 | [COBRA]+ | (AB\|O\|OR)+ |
|:---------------:|:--------:|:----------:|
| <b>(.)+\1   | B        | O          |
| <b>[^ABRC]+ | B        | E          |

Explaination: 
* [COBRA]+ equals 1 or more of a character from `COBRA`
* (AB|O|OR)+ equals 1 or more of a group of `AB` or `O` or `OR`
* (.)+\1 equals backreference to 1 or more of a group of any character except newline e
* [^ABRC]+ equals a 1 or more of a character not from `ABRC` 

### Symbolism

|             | .?.+ | .+ |
|:-----------:|:----:|:-: |
| <b>[*]+ | *    | *  |
| <b>/+   | /    | /  |

Explaination: 
* .?.+ equals 0 or 1 of any character except newline followed by 1 or more of any character except newline
* .+ equals 1 or more of any character except newline
* [*]+ equals 1 or more of the character `*`  
* /+ equals 1 or more `/`  

### Airstrip One

|                 | \d[2480] | 56\|94\|73 |
|:---------------:|:--------:|:--------:|
| <b>18\|19\|20 | *        | *        |
| <b>[6789]\d | /        | /        |

Explaination: 
* \d[2480] equals any digit followed by any digit from `2480` (The result will be a two digit number)
* 56|94|73 equals `56` or `94` or `73`
* 18|19|20 equals `18` or `19` or `20`  
* [6789]\d equals any digit from `6789` followed by any digit (The result will be a two digit number)  
