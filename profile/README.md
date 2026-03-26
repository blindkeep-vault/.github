# BlindKeep

Zero-knowledge digital vault for secure file storage, sharing, inheritance planning, and document notarization.

All encryption happens client-side — the server never sees plaintext data or master keys.

## Open-source components

| Repository | Description |
|---|---|
| [vault-core](https://github.com/blindkeep-vault/vault-core) | Cryptographic primitives — Argon2, ChaCha20-Poly1305, X25519, HKDF, Ed25519 |
| [vault-cli](https://github.com/blindkeep-vault/vault-cli) | Command-line client for drops, notarization, and certificate verification |
| [vault-wasm](https://github.com/blindkeep-vault/vault-wasm) | WebAssembly bindings for browser-side crypto |
| [vault-python](https://github.com/blindkeep-vault/vault-python) | Python SDK — PyO3 crypto bindings and sync/async API client |

## Cryptography

- **XChaCha20-Poly1305** — Authenticated encryption
- **X25519** — Asymmetric key exchange for grant sharing
- **Argon2id** — Password-based key derivation (64 MiB, 3 iterations)
- **HKDF-SHA256** — Subkey derivation
- **Ed25519** — Notarization signatures (strict verification)
- **SHA-256** — Merkle tree hashing

## License

Open-source components are dual-licensed under [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) and [MIT](https://opensource.org/licenses/MIT).
