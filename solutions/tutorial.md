### The OR Symbol

|                 | A&#124;B |
|:---------------:|:--------:|
| <b>A\|Z | A        |

Explanation:
* A&#124;Z equals `A` or `Z`
* A&#124;B equals `A` or `B`

### A Range of characters

|               | [ABC] |
|:-------------:|:-----:|
| <b>[BDF] | B     |

Explanation:
* \[ABC\] equals 1 or more of the letters of  `ABC`
* \[BDF\] equals 1 or more of the letters of  `BDF`


### Characters NOT to include

|                | \[^AB\] |
|:--------------:|:-------:|
| <b>\[ABC\] | C       |

Explanation:
* \[^AB\] equals letters except `A` and `B`
* \[BDF\] equals 1 or more of the letters of `ABC`

### Zero or more

|             | A\*      |
|:-----------:|:--------:|
| <b>A   | A        |
| <b>AB\* | A        |

Explanation:
* A\* equals 0 or more `A`
* A equals `A`
* AB\* equals `A` followed by 0 or more `B`

### Zero or one

|            | A?B? |
|:----------:|:----:|
| <b>A|C | A    |
| <b>B   | B    |

Explanation:
* A?B? equals 0 or more `A` and 0 or more `B`
* A|C equals `A` or `C`
* B equals `B`  
  
### One or more

|            | A+ |
|:----------:|:--:|
| <b>A|B | A  |
| <b>A|Z | A  |

Explanation:
* A+ equals 1 or more `A`
* A|B equals `A` or `B`
* A|Z equals `A` or `Z`   
  
### Backreference

|            | (A)\1 |
|:----------:|:-----:|
| <b>A\|B | A     |
| <b>A\|B | A     |

Explanation:
* (A)\1 equals backreference to group `(A)`
* A|B equals `A` or `B`
* A|B equals `A` or `B`

### Specific amount

|             | A{2,} |
|:-----------:|:-----:|
| <b>A{1} | A     |
| <b>B\|A  | A     |

Explanation:
* (A)\1 equals only 2 or more `A`
* A{1} equals only 1 `A`
* B|A equals `B` or `A`

### Space

|           | A\|\s |
|:---------:|:----:|
| <b>\s | \s   |

Explanation:
* A|\s equals `A` or `Space`
* \s equals `Space`