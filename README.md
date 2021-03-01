# TEd v1.2

TEd is a customisation of [the kilo editor](https://github.com/antirez/kilo).

### Changelog

#### v1 : Bugfixing
0. Used [kilo.c](https://raw.githubusercontent.com/antirez/kilo/master/kilo.c), renamed to TEd
1. Added `system("clear")` to clear screen upon exit 
2. Added `#define`, `#include`, `#ifdef` , `#endif` , `#ifndef`, `#pragma` keywords.
3. Added [#75](https://github.com/antirez/kilo/pull/75/files)
4. Added [#74](https://github.com/antirez/kilo/pull/74)
5. Added [#73](https://github.com/antirez/kilo/pull/73)
6. Added [#72](https://github.com/antirez/kilo/pull/72)
7. Added [#20](https://github.com/antirez/kilo/pull/20)
8. Added [#19](https://github.com/antirez/kilo/pull/19)
9. Added [#17](https://github.com/antirez/kilo/pull/17)

#### v1.1 : Touch-up
0. Used TEd.c (v1)
1. Converted `editorSave()` to use `FILE *` rather than file descriptors.
2. Added [#27](https://github.com/antirez/kilo/pull/27/files)

#### v1.2 : Initial Customization
0. Used TEd (v1.1)
1. Converted many `int`s to standard integers : `uint_fast64_t`, `uint_fast8_t`, etc. Accordingly changed format specifiers.
2. Corrected spellings in comments
3. Added an if `if(ptr == NULL)` check with `fpritf(stderr,"...")` and `exit(1)` for *every* `malloc()` and `realloc()` call. Note the `exit(1)` is *not ideal* and will be improved *soon*.
4. Slightly Changed some printing to be more appropriate/verbose.
5. Changed number of keypresses required to _abandon-exit_ from 3 to 1.

###### Note : TEd is just as alpha , if not _more_ than kilo. Any pull requests, issues, etc. are welcome , and stability or predictability is not guaranteed. However, TEd is **actively maintained**, and so will be fixed _ASAP_ if an issue if discovered, so it "_works_" to the best of my knowledge in the latest release.
