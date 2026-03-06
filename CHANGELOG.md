# Changelog

## Unreleased

### Features

- **`absorb` Command**: New command that analyzes a Terraform plan JSON file to detect drift and automatically generates a graft manifest (`absorb.graft.hcl`) with override blocks to match the current remote state. Supports provider schema for improved output accuracy.
- **Deep Merge for Nested Blocks**: Override files now perform deep merge on nested blocks, preserving original attributes from the source while applying override values. This applies to both static blocks and dynamic blocks.

## [1.1.1](https://github.com/CloudNationHQ/az-cn-go-graft/compare/v1.1.0...v1.1.1) (2026-03-06)


### Bug Fixes

* graft paths and release ([#10](https://github.com/CloudNationHQ/az-cn-go-graft/issues/10)) ([ce505e3](https://github.com/CloudNationHQ/az-cn-go-graft/commit/ce505e3e71d47b6516c59ac886ee81e4f8251d29))

## [1.1.0](https://github.com/CloudNationHQ/az-cn-go-graft/compare/v1.0.1...v1.1.0) (2026-03-06)


### Features

* add step to release go module ([#8](https://github.com/CloudNationHQ/az-cn-go-graft/issues/8)) ([3573024](https://github.com/CloudNationHQ/az-cn-go-graft/commit/3573024f617b86a6b85b05e19b0e6893ebd5e77d))

## [1.0.1](https://github.com/CloudNationHQ/az-cn-go-graft/compare/v1.0.0...v1.0.1) (2026-03-06)


### Bug Fixes

* graft paths ([#5](https://github.com/CloudNationHQ/az-cn-go-graft/issues/5)) ([9c0acb4](https://github.com/CloudNationHQ/az-cn-go-graft/commit/9c0acb48c895dc9cc3e1b9e66e0806a013fc38e2))
* point henglu paths to cloudnation ([#7](https://github.com/CloudNationHQ/az-cn-go-graft/issues/7)) ([a36337b](https://github.com/CloudNationHQ/az-cn-go-graft/commit/a36337b86d9e38217787eb133e54d8f666b05906))

## 1.0.0 (2026-02-11)


### Features

* initial commit ([#1](https://github.com/CloudNationHQ/az-cn-go-graft/issues/1)) ([4be5f4e](https://github.com/CloudNationHQ/az-cn-go-graft/commit/4be5f4e0aea031bef19dc6b6f32f2279aeef93e6))

## v0.1.0

### Features

- Initial release of Graft - The Overlay Engine for Terraform
- `graft build` command to apply patches to Terraform modules
- `graft clean` command to clean up generated files
- `graft scaffold` command to generate manifest files from existing modules
