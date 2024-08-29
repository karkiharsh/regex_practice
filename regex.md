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

**`\w`**

- Matches any word character (letters, digits, and underscores).


**`a{2,4}`**

- Matches `a` repeated between 2 and 4 times.


**`(abc|def)`**

- Matches either `abc` or `def`.
