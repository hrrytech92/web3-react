# `web3-react` 🧰

[![CI](https://github.com/NoahZinsmeister/web3-react/actions/workflows/CI.yml/badge.svg)](https://github.com/NoahZinsmeister/web3-react/actions/workflows/CI.yml)

Warning: alpha code!

Tasks:
- Other Connectors
  - Frame
  - WalletLink
  - WalletConnect V2
  - Gnosis Safe
  - Other injected connectors?
- Address remaining TODOs in the code
- Tests
- Ensure dist/ files can be consumed in e.g. CRA
- Host example/ on CodeSandbox
- Work on DevEx
- Docs
- Upgrade to Node 16 once LTS

## Packages

<details>
  <summary>Expand</summary>

| Package                     | `@alpha` Version                                                                                                                            | Size                                                                                                                                                           | Description |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| `@web3-react/store`         | [![npm](https://img.shields.io/npm/v/@web3-react/store/alpha.svg)](https://www.npmjs.com/package/@web3-react/store/v/alpha)                 | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/store/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/store@alpha)                 |             |
| `@web3-react/types`         | [![npm](https://img.shields.io/npm/v/@web3-react/types/alpha.svg)](https://www.npmjs.com/package/@web3-react/types/v/alpha)                 | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/types/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/types@alpha)                 |             |
| `@web3-react/core`          | [![npm](https://img.shields.io/npm/v/@web3-react/core/alpha.svg)](https://www.npmjs.com/package/@web3-react/core/v/alpha)                   | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/core/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/core@alpha)                   |             |
| **Connectors**              |                                                                                                                                             |                                                                                                                                                                |             |
| `@web3-react/network`       | [![npm](https://img.shields.io/npm/v/@web3-react/network/alpha.svg)](https://www.npmjs.com/package/@web3-react/network/v/alpha)             | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/network/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/network@alpha)             |             |
| `@web3-react/metamask`      | [![npm](https://img.shields.io/npm/v/@web3-react/metamask/alpha.svg)](https://www.npmjs.com/package/@web3-react/metamask/v/alpha)           | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/metamask/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/metamask@alpha)           |             |
| `@web3-react/walletconnect` | [![npm](https://img.shields.io/npm/v/@web3-react/walletconnect/alpha.svg)](https://www.npmjs.com/package/@web3-react/walletconnect/v/alpha) | [![minzip](https://img.shields.io/bundlephobia/minzip/@web3-react/walletconnect/alpha.svg)](https://bundlephobia.com/result?p=@web3-react/walletconnect@alpha) |             |
</details>

## Getting Started

- `yarn`
- `yarn bootstrap`
- `yarn start`

In addition to compiling each package in watch mode, this will also spin up an example app on [http://localhost:3000/](http://localhost:3000/).

## Useful Commands

### Add a dependency

- `yarn lerna add <DEPENDENCY> --scope <SUBPACKAGE>`

### Remove a dependency

- Delete the relevant `package.json` entry

Because of a [lerna bug](https://github.com/lerna/lerna/issues/1883), it's not possible to prune `yarn.lock` programmatically, so regenerate it manually:

- `rm -f packages/<SUBPACKAGE>/yarn.lock`
- `yarn clean --scope SUBPACKAGE`
- `yarn bootstrap`
