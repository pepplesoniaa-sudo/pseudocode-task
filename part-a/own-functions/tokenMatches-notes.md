Saved (local time): 2026-10-16 21:34:57 +01:00

1. My notes on the four Node.js methods
These notes are based on the official Node.js Crypto documentation.
createHash(): Create the fingerprint machine
What it needs: The name of a supported hashing algorithm, such as 'sha256'.
What it returns: A Hash object that can process data and produce a fingerprint.
What happens if the input is wrong? If the algorithm is misspelled or unsupported, Node.js throws an error instead of creating the hash. The algorithms available depend on the Node.js and OpenSSL environment. 




update(): Feed the data into the machine
What it needs: Data in the form of text, a Buffer, a TypedArray, or a DataView. Text uses UTF-8 encoding by default.
What it returns: The same hash object, so another operation can be chained onto it.
What happens if the input is wrong? An unsupported data type or invalid encoding causes an error. You also cannot continue updating a hash after its digest() method has been called. 





digest(): Produce the fingerprint
What it needs: The data previously supplied through update(). It can optionally accept an output encoding, such as 'hex'.
What it returns: A Buffer by default, or a string when an encoding is supplied.
What happens if the input is wrong? An invalid encoding causes an error. You can only finalise a hash once; calling digest() again on the same hash object throws an error. 




timingSafeEqual(): Compare two fingerprints
What it needs: Two supported byte-based inputs, such as Buffer objects, with exactly the same number of bytes.
What it returns: true if their underlying bytes match and false if they do not.
What happens if the input is wrong? If the inputs have different byte lengths, Node.js throws an error instead of returning false. Unsupported input types also cause an error. The comparison uses a constant-time algorithm, but that does not automatically make the surrounding code timing-safe. 





2. Your two reading questions
Question	Answer in my own words
How long is a SHA-256 fingerprint?	It is always 32 bytes, or 256 bits, whether the original text contains one character or a thousand. If displayed as hexadecimal text, it becomes 64 characters. 


What does timingSafeEqual() require?	It needs two supported byte-based inputs with exactly the same byte length. If their lengths differ, it throws an error. 
