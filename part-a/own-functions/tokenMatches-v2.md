Timestamp:2026-10-17 19:08:37 +01:00



FUNCTION tokenMatches



INPUTS:

\- given: any kind of value (text, number, nothing at all). It is the word the visitor supplied.

\- expected: text. It is the real secret word.



OUTPUT:

\- returns false when given is not a string, so the function exits before hashing.

\- returns false when hashing succeeds but the two SHA-256 digest byte sequences do not match.

\- returns true when hashing succeeds and the two SHA-256 digest byte sequences match.



SIDE EFFECTS:



FAILS WHEN:

Returns a value



\- Returns `false` before hashing if `given` is not a string.

\- Returns `false` after hashing if the two digest values are different.

\- Returns `true` after hashing if the two digest values match.



STEPS:



CONFIRMED FROM CODE:

\- Line 14 ends with .digest() with empty brackets, so no encoding is passed.

\- According to my digest() notes, that returns a Buffer (raw bytes), not a hex string.

\- A SHA-256 result is always 32 bytes, whatever length of text went in.

