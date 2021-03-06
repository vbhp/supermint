# crypto

crypto is the cryptographic package adapted for Supermint's uses

## Importing it

To get the interfaces,
`import "github.com/vbhp/supermint/crypto"`

For any specific algorithm, use its specific module e.g.
`import "github.com/vbhp/supermint/crypto/ed25519"`

## Binary encoding

For Binary encoding, please refer to the [Supermint encoding specification](https://docs.supermint.com/master/spec/blockchain/encoding.html).

## JSON Encoding

JSON encoding is done using supermint's internal json encoder. For more information on JSON encoding, please refer to [Supermint JSON encoding](https://github.com/vbhp/supermint/blob/ccc990498df70f5a3df06d22476c9bb83812cbe3/libs/json/doc.go)

```go
Example JSON encodings:

ed25519.PrivKey     - {"type":"supermint/PrivKeyEd25519","value":"EVkqJO/jIXp3rkASXfh9YnyToYXRXhBr6g9cQVxPFnQBP/5povV4HTjvsy530kybxKHwEi85iU8YL0qQhSYVoQ=="}
ed25519.PubKey      - {"type":"supermint/PubKeyEd25519","value":"AT/+aaL1eB0477Mud9JMm8Sh8BIvOYlPGC9KkIUmFaE="}
sr25519.PrivKeySr25519   - {"type":"supermint/PrivKeySr25519","value":"xtYVH8UCIqfrY8FIFc0QEpAEBShSG4NT0zlEOVSZ2w4="}
sr25519.PubKeySr25519    - {"type":"supermint/PubKeySr25519","value":"8sKBLKQ/OoXMcAJVxBqz1U7TyxRFQ5cmliuHy4MrF0s="}
crypto.PrivKeySecp256k1   - {"type":"supermint/PrivKeySecp256k1","value":"zx4Pnh67N+g2V+5vZbQzEyRerX9c4ccNZOVzM9RvJ0Y="}
crypto.PubKeySecp256k1    - {"type":"supermint/PubKeySecp256k1","value":"A8lPKJXcNl5VHt1FK8a244K9EJuS4WX1hFBnwisi0IJx"}
```
