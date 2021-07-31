# [Regex Crossword](https://regexcrossword.com/) Solutions with Explanations 

## Instructions 

Similar to a sudoku puzzle, fill in the blanks with letters that both satisfy the row and column it corresponds to.

### Tutorial

#### The OR Symbol

|                 | A&#124;B |
|:---------------:|:--------:|
| <b>A&#124;Z</b> | A        |

Explaination: 
* A&#124;Z equals `A` or `Z`
* A&#124;B equals `A` or `B`

#### A Range of characters

|               | [ABC] |
|:-------------:|:-----:|
| <b>[BDF]<\b>  | B     |

Explaination: 
* \[ABC\] equals 1 or more of the letters of  `ABC`
* \[BDF\] equals 1 or more of the letters of  `BDF`


#### Charactrs NOT to include

|                | \[^AB\] |
|:--------------:|:-------:|
| <b>\[ABC\]<\b> | C       |

Explaination: 
* \[^AB\] equals letters except `A` and `B`
* \[BDF\] equals 1 or more of the letters of `ABC`

#### Zero or more

|             | A\*      |
|:-----------:|:--------:|
| <b>A<\b>    | A        |
| <b>AB\*<\b> | A        |

Explaination: 
* A\* equals 0 or more `A`
* A equals `A`
* AB\* equals `A` followed by 0 or more `B`

#### Zero or one

|            | A?B? |
|:----------:|:----:|
| <b>A|C<\b> | A    |
| <b>B<\b>   | B    |

Explaination: 
* A?B? equals 0 or more `A` and 0 or more `B`
* A|C equals `A` or `C`
* B equals `B`  
  
#### One or more

|            | A+ |
|:----------:|:--:|
| <b>A|B<\b> | A  |
| <b>A|Z<\b> | A  |

Explaination: 
* A+ equals 1 or more `A`
* A|B equals `A` or `B`
* A|Z equals `A` or `Z`   
  
#### Backreference

|            | (A)\1 |
|:----------:|:-----:|
| <b>A|B<\b> | A     |
| <b>A|B<\b> | A     |

Explaination: 
* (A)\1 equals backreference to group `(A)`
* A|B equals `A` or `B`
* A|B equals `A` or `B`

#### Specific amount

|             | A{2,} |
|:-----------:|:-----:|
| <b>A{1}<\b> | A     |
| <b>B|A<\b>  | A     |

Explaination: 
* (A)\1 equals only 2 or more `A`
* A{1} equals only 1 `A`
* B|A equals `B` or `A`

#### Space

|           | A|\s |
|:---------:|:----:|
| <b>\s<\b> | \s   |

Explaination: 
* A|\s equals `A` or `Space`
* \s equals `Space`

## For More Regex Resources


[RegExr: Learn, Build, & Test RegEx](https://regexr.com/)
