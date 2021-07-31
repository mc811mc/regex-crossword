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
* \[ABC\] equals one or more of the letters of  `ABC`
* \[BDF\] equals one or more of the letters of  `BDF`


#### Charactrs NOT to include

|                | \[^AB\] |
|:--------------:|:-------:|
| <b>\[ABC\]<\b> | C       |

Explaination: 
* \[^AB\] equals letters except `A` and `B`
* \[BDF\] equals one or more of the letters of `ABC`

#### Zero or more

|             | A\*      |
|:-----------:|:--------:|
| <b>A<\b>    | A        |
| <b>AB\*<\b> | A        |

Explaination: 
* A\* equals zero or more `A`
* A equals `A`
* AB\* equals `A` followed by zero or more `B`

## For More Regex Resources


[RegExr: Learn, Build, & Test RegEx](https://regexr.com/)
