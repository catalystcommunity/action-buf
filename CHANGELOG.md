# [1.1.0](https://github.com/catalystcommunity/action-buf/compare/v1.0.15...v1.1.0) (2023-12-05)


### Features

* implement working-directory, breaking-against, commit, registry-login inputs ([#26](https://github.com/catalystcommunity/action-buf/issues/26)) ([858d352](https://github.com/catalystcommunity/action-buf/commit/858d352afc4cc515eb4172cc7b4e2f2cb5766b8f))

## [1.0.15](https://github.com/catalystcommunity/action-buf/compare/v1.0.14...v1.0.15) (2023-09-29)


### Bug Fixes

* Update checkout and setup-go versions, update go version to 1.21, remove cache that is now included in setup-go ([#25](https://github.com/catalystcommunity/action-buf/issues/25)) ([df3f723](https://github.com/catalystcommunity/action-buf/commit/df3f723832f941f2f89b8cfbc2f605cb66fc77b1))

## [1.0.14](https://github.com/catalystcommunity/action-buf/compare/v1.0.13...v1.0.14) (2023-06-06)


### Bug Fixes

* remove skip-ci from default commit message ([#24](https://github.com/catalystcommunity/action-buf/issues/24)) ([1b9a128](https://github.com/catalystcommunity/action-buf/commit/1b9a1283b5f0ade452e774b2197c5bf7f34434ea))

## [1.0.13](https://github.com/catalystcommunity/action-buf/compare/v1.0.12...v1.0.13) (2023-03-29)


### Bug Fixes

* Modify default commit message to use language that will not create new runs when generate commits generated code ([#22](https://github.com/catalystcommunity/action-buf/issues/22)) ([c970f75](https://github.com/catalystcommunity/action-buf/commit/c970f75ddca355ff018f4033ee5c24c24754e746))

## [1.0.12](https://github.com/catalystcommunity/action-buf/compare/v1.0.11...v1.0.12) (2022-12-08)


### Bug Fixes

* Update buf setup action version, move bsr login up in the steps ([#21](https://github.com/catalystcommunity/action-buf/issues/21)) ([3efb211](https://github.com/catalystcommunity/action-buf/commit/3efb211118ddeb404a0ded1a18a7065c104ebeb0))

## [1.0.11](https://github.com/catalystcommunity/action-buf/compare/v1.0.10...v1.0.11) (2022-10-05)


### Bug Fixes

* update catalystcommunity go-proto-gql version to gain suffix support ([#19](https://github.com/catalystcommunity/action-buf/issues/19)) ([bc2b482](https://github.com/catalystcommunity/action-buf/commit/bc2b482a910c93eb2723397728dd9ce5d6ffccd6))

## [1.0.10](https://github.com/catalystcommunity/action-buf/compare/v1.0.9...v1.0.10) (2022-09-08)


### Bug Fixes

* update gql gen commit hash ([#18](https://github.com/catalystcommunity/action-buf/issues/18)) ([57f3485](https://github.com/catalystcommunity/action-buf/commit/57f3485b22d12e9924de633977a2c52a382d5536))

## [1.0.9](https://github.com/catalystcommunity/action-buf/compare/v1.0.8...v1.0.9) (2022-08-30)


### Bug Fixes

* Bump @actions/core from 1.6.0 to 1.9.1 ([#16](https://github.com/catalystcommunity/action-buf/issues/16)) ([d4ac78f](https://github.com/catalystcommunity/action-buf/commit/d4ac78fb807e5cb0743b7bcdc2f3c945862d2a66))
* Enhanced gql generation ([#17](https://github.com/catalystcommunity/action-buf/issues/17)) ([0fa01f6](https://github.com/catalystcommunity/action-buf/commit/0fa01f6c35d980dfaced55d0ad7552ef37c57256))

## [1.0.8](https://github.com/catalystcommunity/action-buf/compare/v1.0.7...v1.0.8) (2022-08-15)


### Bug Fixes

* Make default commit message ci friendly. If it includes language that causes ci to not run then it doesn't run even when things are squash merged, so it won't work at all. ([#15](https://github.com/catalystcommunity/action-buf/issues/15)) ([c6c7231](https://github.com/catalystcommunity/action-buf/commit/c6c72314a3ce8ac774d10857fcd1380915cb9e8e))

## [1.0.7](https://github.com/catalystcommunity/action-buf/compare/v1.0.6...v1.0.7) (2022-08-13)


### Bug Fixes

* Add configurable commit message ([#14](https://github.com/catalystcommunity/action-buf/issues/14)) ([0d43f6d](https://github.com/catalystcommunity/action-buf/commit/0d43f6dcd5615600cb8d952ac574136ffa58df18))

## [1.0.6](https://github.com/catalystcommunity/action-buf/compare/v1.0.5...v1.0.6) (2022-05-23)


### Bug Fixes

* Use forked version of protobuf-ts, and use protoc-gen-gql pinned to a git hash that has better support for protobuf uptional fields ([#13](https://github.com/catalystcommunity/action-buf/issues/13)) ([d6085c8](https://github.com/catalystcommunity/action-buf/commit/d6085c8dc9a7fa3e6bd28808c2f182581a89dbaf))

## [1.0.5](https://github.com/catalystcommunity/action-buf/compare/v1.0.4...v1.0.5) (2022-05-17)


### Bug Fixes

* Allow proto-loader configuration with sensible default that includes keepCase to keep the proto casing. ([#12](https://github.com/catalystcommunity/action-buf/issues/12)) ([f57902b](https://github.com/catalystcommunity/action-buf/commit/f57902bada161c0f906987614400db9dd6ee2862))

## [1.0.4](https://github.com/catalystcommunity/action-buf/compare/v1.0.3...v1.0.4) (2022-04-14)


### Bug Fixes

* Create the directory first, then copy ([#11](https://github.com/catalystcommunity/action-buf/issues/11)) ([1e4e5fe](https://github.com/catalystcommunity/action-buf/commit/1e4e5fe509e85de46bb11469c43627fbacad9b47))

## [1.0.3](https://github.com/catalystcommunity/action-buf/compare/v1.0.2...v1.0.3) (2022-04-14)


### Bug Fixes

* Copy the .proto file, it's necessary for typescript clients ([#10](https://github.com/catalystcommunity/action-buf/issues/10)) ([6674459](https://github.com/catalystcommunity/action-buf/commit/6674459b5c097c01d87ec09f40e861688e622855))

## [1.0.2](https://github.com/catalystcommunity/action-buf/compare/v1.0.1...v1.0.2) (2022-04-14)


### Bug Fixes

* Enhanced typescript support ([#9](https://github.com/catalystcommunity/action-buf/issues/9)) ([6acea6e](https://github.com/catalystcommunity/action-buf/commit/6acea6e9341aade9db38469ff87faf49eed2b2cc))

## [1.0.1](https://github.com/catalystcommunity/action-buf/compare/v1.0.0...v1.0.1) (2022-04-12)


### Bug Fixes

* Add support for generating graphql types via https://github.com/danielvladco/go-proto-gql ([#8](https://github.com/catalystcommunity/action-buf/issues/8)) ([c7a78cc](https://github.com/catalystcommunity/action-buf/commit/c7a78cccee52867a360bd3bb4ae494bf2ea053ff))

# 1.0.0 (2022-04-01)


### Bug Fixes

* Fix package.json url ([#6](https://github.com/catalystcommunity/action-buf/issues/6)) ([5553400](https://github.com/catalystcommunity/action-buf/commit/5553400ce329b431068be01f5567475af6cd0242))
* Initial commit ([#1](https://github.com/catalystcommunity/action-buf/issues/1)) ([c550696](https://github.com/catalystcommunity/action-buf/commit/c550696ab42a67a81f087b4018710218b49c446a))
* Release ([#3](https://github.com/catalystcommunity/action-buf/issues/3)) ([07397bb](https://github.com/catalystcommunity/action-buf/commit/07397bbafe3274efa30279dbed2e048b4a0d33e6))
* Release ([#4](https://github.com/catalystcommunity/action-buf/issues/4)) ([c746d4c](https://github.com/catalystcommunity/action-buf/commit/c746d4c1688539939d8fb04a9faa461dc6b89782))
* Release ([#5](https://github.com/catalystcommunity/action-buf/issues/5)) ([e1c2cfb](https://github.com/catalystcommunity/action-buf/commit/e1c2cfb8a797f23522bbff52d9cc023bf3e52963))
* Release ([#7](https://github.com/catalystcommunity/action-buf/issues/7)) ([61bf989](https://github.com/catalystcommunity/action-buf/commit/61bf989aa2c667707cb35a3ff6afb16ce063a779))

# 1.0.0 (2022-02-28)


### Bug Fixes

* Initial commit ([#1](https://github.com/catalystcommunity/action-composite-action-template/issues/1)) ([3bcf298](https://github.com/catalystcommunity/action-composite-action-template/commit/3bcf298630471c46d9f9a1f3a24c2c15342e1855))
