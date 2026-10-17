`tokenMatches` — v1 pseudocode
FUNCTION
`tokenMatches(given, expected)` checks whether the supplied value matches the expected token by comparing their SHA-256 digests.
INPUTS

* `given`: Any kind of value. The function must check whether it is a string before hashing it.
* `expected`: The expected token, declared as a string.

OUTPUT

* A boolean: `true` when the two digest values match, or `false` when they do not.
* If `given` is not a string, it returns `false` immediately without hashing either value.

SIDE EFFECTS

* No externally visible side effects are intended. The function hashes the inputs and compares the resulting values; it does not intentionally change either input.
* Any additional side effects would depend on how the `sha256` helper is implemented.

FAILS WHEN
Returns a value

* Early exit — invalid `given` type: If `given` is not a string, return `false` immediately.
* If `given` is a string and both digest values are produced successfully, return `true` when the digest bytes match and `false` when they do not.

Throws

* Hash creation or hashing can throw if the `sha256` helper uses an unsupported algorithm, invalid data or encoding, or an already-finalised hash object. The helper implementation is not shown, so its exact failure cases need to be checked.
* `timingSafeEqual()` can throw if either value it receives is not a supported byte-based type, or if the two values have different byte lengths. The helper implementation is not shown, so this cannot be confirmed from `tokenMatches` alone.
