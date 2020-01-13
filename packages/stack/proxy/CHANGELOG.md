# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [5.0.0](https://github.com/embark-framework/embark/compare/v5.0.0-beta.0...v5.0.0) (2020-01-07)

**Note:** Version bump only for package embark-proxy





# [5.0.0-alpha.9](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.8...v5.0.0-alpha.9) (2019-12-20)


### Build System

* **deps:** bump web3[-*] from 1.2.1 to 1.2.4 ([7e550f0](https://github.com/embark-framework/embark/commit/7e550f0))


### BREAKING CHANGES

* **deps:** bump embark's minimum supported version of parity from
`>=2.0.0` to `>=2.2.1`. This is necessary since web3 1.2.4 makes use of the
`eth_chainId` RPC method (EIP 695) and that parity version is the earliest one
to implement it.

[bug]: https://github.com/ethereum/web3.js/issues/3283





# [5.0.0-alpha.8](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.7...v5.0.0-alpha.8) (2019-12-19)

**Note:** Version bump only for package embark-proxy





# [5.0.0-alpha.5](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.4...v5.0.0-alpha.5) (2019-12-16)


### Bug Fixes

* fix node connection test to use the endpoints correctly ([0503bb2](https://github.com/embark-framework/embark/commit/0503bb2))





# [5.0.0-alpha.4](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.3...v5.0.0-alpha.4) (2019-12-12)


### Bug Fixes

* **@embark/proxy:** fix conflict for WS port in the proxy ([eae97de](https://github.com/embark-framework/embark/commit/eae97de))
* **@embark/test:** fix using --node option in tests ([b82a240](https://github.com/embark-framework/embark/commit/b82a240))





# [5.0.0-alpha.3](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.2...v5.0.0-alpha.3) (2019-12-06)

**Note:** Version bump only for package embark-proxy





# [5.0.0-alpha.2](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.1...v5.0.0-alpha.2) (2019-12-05)


### Bug Fixes

* **@embark/proxy:** Fix unsubsribe handling and add new provider ([f6f4507](https://github.com/embark-framework/embark/commit/f6f4507))


### Features

* **@embark/embark-rpc-manager:** Add support for `eth_signTypedData_v3` ([c7ec49a](https://github.com/embark-framework/embark/commit/c7ec49a)), closes [#1850](https://github.com/embark-framework/embark/issues/1850) [#1850](https://github.com/embark-framework/embark/issues/1850)





# [5.0.0-alpha.1](https://github.com/embark-framework/embark/compare/v5.0.0-alpha.0...v5.0.0-alpha.1) (2019-11-05)


### Bug Fixes

* **@embark/proxy:** Fix contract event subscriptions ([f9ad486](https://github.com/embark-framework/embark/commit/f9ad486))
* fix ws providers to have the patch for a bigger threshold ([#2017](https://github.com/embark-framework/embark/issues/2017)) ([9e654c5](https://github.com/embark-framework/embark/commit/9e654c5))





# [5.0.0-alpha.0](https://github.com/embark-framework/embark/compare/v4.1.1...v5.0.0-alpha.0) (2019-10-28)


### Bug Fixes

* fix error logs in the cockpit due from negative blocks numbers ([#1967](https://github.com/embark-framework/embark/issues/1967)) ([4b947bb](https://github.com/embark-framework/embark/commit/4b947bb))
* **@embark/proxy:** Check if WebSocket open before sending ([#1978](https://github.com/embark-framework/embark/issues/1978)) ([db71a93](https://github.com/embark-framework/embark/commit/db71a93))
* **@embark/proxy:** Fix contract event subscriptions ([173d53d](https://github.com/embark-framework/embark/commit/173d53d))


### Build System

* bump all packages' engines settings ([#1985](https://github.com/embark-framework/embark/issues/1985)) ([ed02cc8](https://github.com/embark-framework/embark/commit/ed02cc8))


### Features

* **@embark/test-runner:** make vm default node ([#1846](https://github.com/embark-framework/embark/issues/1846)) ([f54fbf0](https://github.com/embark-framework/embark/commit/f54fbf0))
* call action before starting the blockchain node ([c54b8d9](https://github.com/embark-framework/embark/commit/c54b8d9))


### BREAKING CHANGES

* node: >=10.17.0 <12.0.0
npm: >=6.11.3
yarn: >=1.19.1

node v10.17.0 is the latest in the 10.x series and is still in the Active LTS
lifecycle. Embark is still not compatible with node's 12.x and 13.x
series (because of some dependencies), otherwise it would probably make sense
to bump our minimum supported node version all the way to the most recent 12.x
release.

npm v6.11.3 is the version that's bundled with node v10.17.0.

yarn v1.19.1 is the most recent version as of the time node v10.17.0 was
released.