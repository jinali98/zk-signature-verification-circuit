# ZK Signature Verification Circuit

This project implements a zero-knowledge signature verification circuit using the ecrecover functionality.

## Setup

### 1. Generate Hashed Message

To create a hashed message for testing:

```bash
cast keccak "hello world"
```

### 2. Setup Local Wallet for Testing

Import a wallet locally (this will prompt for private key and password):

```bash
cast wallet import jinali --interactive
```

List available wallets:

```bash
cast wallet list
```

Get the wallet address:

```bash
cast wallet address --account jinali
```

Get the wallet's public key:

```bash
cast wallet public-key --account jinali
```

**Note:** The public key returned from the above command needs to be split into x and y components for use in the circuit.
