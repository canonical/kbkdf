# Description
This package implements the key derivation functions defined in [NIST SP800-108](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-108.pdf).

It implements the 3 modes specified:
- Counter mode
- Feedback mode (with or without iteration counter)
- Double-Pipeline mode (with or without iteration counter)

It includes a sub-package implementing various HMAC based pseudo-random functions.

The counter mode KDF with HMAC based PRF is used in the [TPM 2.0 Reference Library specification](https://trustedcomputinggroup.org/resource/tpm-library-specification/) and consumed by the [Go TPM2 package](https://github.com/canonical/go-tpm2/)