## [1.0.8](https://github.com/catalystsquad/action-buf/compare/v1.0.7...v1.0.8) (2022-08-15)


### Bug Fixes

* Make default commit message ci friendly. If it includes language that causes ci to not run then it doesn't run even when things are squash merged, so it won't work at all. ([#15](https://github.com/catalystsquad/action-buf/issues/15)) ([c6c7231](https://github.com/catalystsquad/action-buf/commit/c6c72314a3ce8ac774d10857fcd1380915cb9e8e))

## [1.0.7](https://github.com/catalystsquad/action-buf/compare/v1.0.6...v1.0.7) (2022-08-13)


### Bug Fixes

* Add configurable commit message ([#14](https://github.com/catalystsquad/action-buf/issues/14)) ([0d43f6d](https://github.com/catalystsquad/action-buf/commit/0d43f6dcd5615600cb8d952ac574136ffa58df18))

## [1.0.6](https://github.com/catalystsquad/action-buf/compare/v1.0.5...v1.0.6) (2022-05-23)


### Bug Fixes

* Use forked version of protobuf-ts, and use protoc-gen-gql pinned to a git hash that has better support for protobuf uptional fields ([#13](https://github.com/catalystsquad/action-buf/issues/13)) ([d6085c8](https://github.com/catalystsquad/action-buf/commit/d6085c8dc9a7fa3e6bd28808c2f182581a89dbaf))

## [1.0.5](https://github.com/catalystsquad/action-buf/compare/v1.0.4...v1.0.5) (2022-05-17)


### Bug Fixes

* Allow proto-loader configuration with sensible default that includes keepCase to keep the proto casing. ([#12](https://github.com/catalystsquad/action-buf/issues/12)) ([f57902b](https://github.com/catalystsquad/action-buf/commit/f57902bada161c0f906987614400db9dd6ee2862))

## [1.0.4](https://github.com/catalystsquad/action-buf/compare/v1.0.3...v1.0.4) (2022-04-14)


### Bug Fixes

* Create the directory first, then copy ([#11](https://github.com/catalystsquad/action-buf/issues/11)) ([1e4e5fe](https://github.com/catalystsquad/action-buf/commit/1e4e5fe509e85de46bb11469c43627fbacad9b47))

## [1.0.3](https://github.com/catalystsquad/action-buf/compare/v1.0.2...v1.0.3) (2022-04-14)


### Bug Fixes

* Copy the .proto file, it's necessary for typescript clients ([#10](https://github.com/catalystsquad/action-buf/issues/10)) ([6674459](https://github.com/catalystsquad/action-buf/commit/6674459b5c097c01d87ec09f40e861688e622855))

## [1.0.2](https://github.com/catalystsquad/action-buf/compare/v1.0.1...v1.0.2) (2022-04-14)


### Bug Fixes

* Enhanced typescript support ([#9](https://github.com/catalystsquad/action-buf/issues/9)) ([6acea6e](https://github.com/catalystsquad/action-buf/commit/6acea6e9341aade9db38469ff87faf49eed2b2cc))

## [1.0.1](https://github.com/catalystsquad/action-buf/compare/v1.0.0...v1.0.1) (2022-04-12)


### Bug Fixes

* Add support for generating graphql types via https://github.com/danielvladco/go-proto-gql ([#8](https://github.com/catalystsquad/action-buf/issues/8)) ([c7a78cc](https://github.com/catalystsquad/action-buf/commit/c7a78cccee52867a360bd3bb4ae494bf2ea053ff))

# 1.0.0 (2022-04-01)


### Bug Fixes

* Fix package.json url ([#6](https://github.com/catalystsquad/action-buf/issues/6)) ([5553400](https://github.com/catalystsquad/action-buf/commit/5553400ce329b431068be01f5567475af6cd0242))
* Initial commit ([#1](https://github.com/catalystsquad/action-buf/issues/1)) ([c550696](https://github.com/catalystsquad/action-buf/commit/c550696ab42a67a81f087b4018710218b49c446a))
* Release ([#3](https://github.com/catalystsquad/action-buf/issues/3)) ([07397bb](https://github.com/catalystsquad/action-buf/commit/07397bbafe3274efa30279dbed2e048b4a0d33e6))
* Release ([#4](https://github.com/catalystsquad/action-buf/issues/4)) ([c746d4c](https://github.com/catalystsquad/action-buf/commit/c746d4c1688539939d8fb04a9faa461dc6b89782))
* Release ([#5](https://github.com/catalystsquad/action-buf/issues/5)) ([e1c2cfb](https://github.com/catalystsquad/action-buf/commit/e1c2cfb8a797f23522bbff52d9cc023bf3e52963))
* Release ([#7](https://github.com/catalystsquad/action-buf/issues/7)) ([61bf989](https://github.com/catalystsquad/action-buf/commit/61bf989aa2c667707cb35a3ff6afb16ce063a779))

# 1.0.0 (2022-02-28)


### Bug Fixes

* Initial commit ([#1](https://github.com/catalystsquad/action-composite-action-template/issues/1)) ([3bcf298](https://github.com/catalystsquad/action-composite-action-template/commit/3bcf298630471c46d9f9a1f3a24c2c15342e1855))
