# Uniswap SDK

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![Actions Status](https://github.com/Uniswap/uniswap-sdk/workflows/CI/badge.svg)](https://github.com/Uniswap/uniswap-sdk)
[![npm version](https://img.shields.io/npm/v/@uniswap/sdk/latest.svg)](https://www.npmjs.com/package/@uniswap/sdk/v/latest)
[![npm bundle size (scoped version)](https://img.shields.io/bundlephobia/minzip/@uniswap/sdk/latest.svg)](https://bundlephobia.com/result?p=@uniswap/sdk@latest)

In-depth documentation on this SDK is available at [uniswap.org](https://uniswap.org/docs/v2/SDK/getting-started/).

## Running tests

To run the tests, follow these steps. You must have at least node v10 and [yarn](https://yarnpkg.com/) installed.

First clone the repository:

```sh
git clone https://github.com/Uniswap/uniswap-sdk.git
```

Move into the uniswap-sdk working directory

```sh
cd uniswap-sdk/
```

Install dependencies

```sh
yarn install
```

Run tests

```sh
yarn test
```

You should see output like the following:

```sh
yarn run v1.22.4
$ tsdx test
 PASS  test/constants.test.ts
 PASS  test/pair.test.ts
 PASS  test/fraction.test.ts
 PASS  test/miscellaneous.test.ts
 PASS  test/entities.test.ts
 PASS  test/trade.test.ts

Test Suites: 1 skipped, 6 passed, 6 of 7 total
Tests:       3 skipped, 82 passed, 85 total
Snapshots:   0 total
Time:        5.091s
Ran all test suites.
✨  Done in 6.61s.
```

#修改工厂地址和keccack

将Const/index.ts下面的这个地方改成自己的地址

export const FACTORY_ADDRESS = '0xCfe8160192297d871c288CD5cb8b97F8ffB10E6F'

export const INIT_CODE_HASH = '0x6d15a2b06bcbfdf3e200e48a7b5aa03661215fc068fd0762d44693a554cb5e66'