Saved (local time): 2026-10-16 21:34:57 +01:00

3. Can line 4 ever break?
return timingSafeEqual(sha256(given), sha256(expected));


Think about it in three steps.
1. sha256(given) produces a fingerprint of 32 bytes.
2. sha256(expected) also produces a fingerprint of 32 bytes.
3. timingSafeEqual() receives two fingerprints of equal length.
Conclusion: If sha256() returns a Buffer containing the raw SHA-256 digest in both cases, line 4 will not fail because of a length mismatch. Even if the original words have different lengths, their SHA-256 fingerprints still have the same length.
However, there is an important catch: we have not seen the implementation of sha256(). If it returns hexadecimal strings instead of Buffer objects, timingSafeEqual() will throw because strings are not accepted as its inputs.
There is also a broader security detail: a constant-time comparison does not guarantee that the entire function is constant-time. Hashing and the surrounding code can still introduce timing differences.
