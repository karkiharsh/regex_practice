---
sr-due: 2024-08-23
sr-interval: 1
sr-ease: 230
---

#2024-08-22 #recall 

### basic commands 

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

- Matches either `abc` or `def`.

`(?i)`

- case insensitive matching
- `(?i)\b\b`

---
#2024-09-03
### Daily Use records.

`tree -d -L 1 | grep -oP '(?<=\|-- ).*'`
``tree -d -L 1 | grep -oP '(?<=\|-- ).*' | sed "s|^|\"$(pwd)/|"``

on this string  .

```sample text 

|-- B2B
|-- B2B2
|-- FormsPro
|-- PDFSimpli.Web
|-- PDFSimpli.Web.LP
|-- ServiceBusExplorer
|-- Signsimpli
|-- Test-env
|-- WorkSimpli.Dashboard
|-- WorkSimpli.DashboardOrch
|-- WorkSimpli.DocBuilder
|-- WorkSimpli.DocEditor
|-- WorkSimpli.DocEditor.API
|-- WorkSimpli.DocProfile
|-- WorkSimpli.DocSearchV2
|-- WorkSimpli.PaymentOrchestration
|-- WorkSimpli.ResumeBuild.Web
|-- WorkSimpli.Template.API
|-- anoteer-pdf.js%20source
|-- api_body
|-- formJSONfiles
|-- legalsimpli
|-- pdf-editor
|-- pdf-editor-original
|-- pdfjs-complete
|-- sample images
|-- samplepdfs
`-- templateCilentBackup



```

### With regex you can _count_ the number of matches. Can you make it return the number of uppercase consonants (B,C,D,F,..,X,Y,Z) in a given string? E.g.: it should return `3` with the text `ABcDeFO!`. **Note:** Only ASCII. We consider `Y` to be a consonant!

**Example:** the regex `/./g` will return **3** when run against the string `abc`.

`/[BCDFGHJKLMNPQRSTVWXYZ]/g


### Count the number of integers in a given string. Integers are, for example: `1, 2, 65, 2579`, etc.

`/\d+/g`