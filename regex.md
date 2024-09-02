---
sr-due: 2024-08-23
sr-interval: 1
sr-ease: 230
---

#2024-08-22 #recall 

`a.b`
- matches for any character
- except `newline`

`^prefix`
 - matches for prefix of a string

`suffix$`
- matches for suffix of a string

`cdef*dd`
- 0 or more f

`cd(ef)*dd`
- 0 or more (ef) as this is a system.

**`[abc]`**
  - Matches any one of the characters `a`, `b`, or `c`.

**`\d`**

- Matches any digit (equivalent to `[0-9]`).


`\b`
- this is word boundary

**`\w`**

- Matches any word character (letters, digits, and underscores).
- `\w{3}` -> match exactly 3
- `\b\w{3}\b` -> word boundary

**`a{2,4}`**

- Matches `a` repeated between 2 and 4 times.


**`(abc|def)`**

`(?i)`

- case insensitive matching
- `(?i)\b\b`
- Matches either `abc` or `def`.


//--------------------

use substitution to replace every occurrence of the word i with the word I (uppercase, I as in me). E.g.: i'm replacing it. am i not? -> I'm replacing it. am I not?.

A regex match is replaced with the text in the Substitution field when using substitution.

 -/\b[i]\b/g
 - g for global replacement
