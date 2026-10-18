Timestamp:2026-10-17 19:08:37 +01:00

Edited: 2026-10-18 10:17:52 +01:00

Edited: 2026-10-18 11:01:05 +01:00

Edited: 2026-10-18 16:58:49 +01:00

Edited: 2026-10-18 17:39:28 +01:00

Edited: 2026-10-18 17:51:17 +01:00



FUNCTION tokenMatches



INPUTS:

* given: any kind of value (text, number, nothing at all). It is the word the visitor supplied.
* expected: text. It is the real secret word.



OUTPUT:

* returns false when given is not a string, so the function exits before hashing.
* returns false when hashing succeeds but the two SHA-256 digest byte sequences do not match.
* returns true when hashing succeeds and the two SHA-256 digest byte sequences match.



SIDE EFFECTS:


The function reads `given` and `expected`, hashes their text, compares the two digests, and returns `true` or `false`. It does not modify either input or perform external actions such as logging, writing data, or making network requests.



FAILS WHEN:

Returns a value



* Returns `false` before hashing if `given` is not a string.
* Returns `false` after hashing if the two digest values are different.
* Returns `true` after hashing if the two digest values match.



STEPS:

1. Receive given and expected.
2. Early exit check:
   IF given is not a string
       RETURN false and stop
   OTHERWISE
       continue to step 3
   END IF
3. Turn given into a fingerprint. The result is a buffer of exactly 32 bytes, and the size does not depend on how long the text is..
4. Turn expected into a fingerprint. The result is a buffer of exactly 32 bytes, and the size does not depend on how long the text is..
5. Compare the fingerprints: Compare the two fingerprints from steps 3 and 4. They are raw byte blocks of equal length because steps 3 and 4 each produce exactly 32 bytes. The comparison returns true if all bytes match and false otherwise.
6. Return the boolean produced by the comparison.



CONFIRMED FROM CODE:

* Line 14 ends with .digest() with empty brackets, so no encoding is passed.
* According to my digest() notes, that returns a Buffer (raw bytes), not a hex string.
* A SHA-256 result is always 32 bytes, whatever length of text went in.

