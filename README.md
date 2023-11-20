
## Overview

This repository is a customized version of Go Ethereum (geth) with specific enhancements and modifications. It is tailored to meet particular requirements and includes improvements for a specialized use case.

## Building from Source

To build this custom Ethereum fork, follow the standard build instructions for Go Ethereum. Ensure you have Go (version 1.19 or later) and a C compiler installed. Detailed build instructions are available in the [Installation Instructions](https://geth.ethereum.org/docs/getting-started/installing-geth).

To build `geth`, use the following command:

```shell
make geth
```

For the full suite of utilities:

```shell
make all
```

## Executables

The repository includes various executables found in the `cmd` directory, each serving specific purposes:

- **`geth`**: Main Ethereum CLI client, serving as the entry point into the Ethereum network. It supports various modes (full, archive, light) and provides JSON RPC endpoints for interaction.

- **`clef`**: Stand-alone signing tool, functioning as a backend signer for `geth`.

- **`devp2p`**: Utilities to interact with nodes on the networking layer without running a full blockchain.

- **`abigen`**: Source code generator to convert Ethereum contract definitions into Go packages.

- **`bootnode`**: Stripped-down version of the Ethereum client that participates only in the network node discovery protocol.

- **`evm`**: Developer utility version of the Ethereum Virtual Machine (EVM) for fine-grained debugging of EVM opcodes.

- **`rlpdump`**: Developer utility tool to convert binary RLP (Recursive Length Prefix) dumps to a user-friendly hierarchical representation.

## Running `geth`

Refer to the [CLI Wiki page](https://geth.ethereum.org/docs/fundamentals/command-line-options) for a comprehensive list of command line options. Below are common scenarios:

...

## Contributing

Contributions to this customized Ethereum fork are welcome. Please follow the guidelines in the [Developers' Guide](https://geth.ethereum.org/docs/developers/geth-developer/dev-guide) for setting up your environment, managing dependencies, and testing procedures.

### License

The custom Ethereum fork is licensed under the [GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.en.html) for the library code and [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html) for the binaries. Please review the `COPYING.LESSER` and `COPYING` files in the repository for detailed licensing information.
