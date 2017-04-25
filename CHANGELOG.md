# CHANGELOG
All notable changes to this project will be documented in this file.

## [Unreleased][unreleased]

## [v5.0.0] - 2017-04-25
### Added
- Added `array-bracket-spacing`, `object-curly-spacing`, and `block-spacing` rules as `[true, "always"]`
- Added `handle-callback-err` rule

### Changed
- Upgraded `vrsource-tslint-rules` to `5.1.0`
- Removed `literal-spacing` rule to use the `tslint-eslint-rules` versions that have `--fix` support
- Changed `ext-variable-name` to allow functions with leading underscores
- Changed `ext-variable-name` to enforce camel case on public methods and properties

## [v4.1.0] - 2017-04-24
### Fixed
- Disable no-inferrable-types since the automatic --fix for this rule is broken

### Changed
- Update tslint and rules to 5.1.x.

## [v4.0.0] - 2017-04-24
### Added
- Add `tslint-eslint-rules` dependency to allow for more eslint rules to be used
- Added the following rules from `tslint-eslint-rules`: `no-constant-condition`, `no-duplicate-case`, `no-empty-character-class`, `no-ex-assign`, `no-extra-boolean-cast`, `no-extra-semi`, `no-inner-declarations`, `no-invalid-regexp`, `no-irregular-whitespace`, `no-regex-spaces`, `no-sparse-arrays`, `no-unexpected-multiline`

## [v3.1.2] - 2017-04-20
### Changed
- Removed `ext-variable-name` rule for `"default"`

## [v3.1.1] - 2017-04-20
### Changed
- Removed `ext-variable-name` rule for `"variable"`

### Fixed
- Removed `tslint-eslint-rules` dependency since that isn't being used yet

## [v3.1.0] - 2017-04-20
### Changed
- Removed `conditional-expression-parens` rule
- Removed `ext-variable-name` rule for `"variable", "const"`

### Fixed
- Fixed version of `tslint` that is required by project `^4.5.1`

## [v3.0.1] - 2017-04-20
### Fixed
- Update `README.md` with instructions for including the new `vrsource-tslint-rules` in a project

## [v3.0.0] - 2017-04-20
### Added
- New dependency on rules from `vrsource-tslint-rules`
- Added `conditional-expression-parens`, `dot-notation`, `ext-variable-name`, `literal-spacing`, `multiline-arrow`, `no-duplicate-imports`, and `prefer-literal` rules from `vrsource-tslint-rules` to `tslint-base.json`

## [v2.0.0] - 2017-04-19
### Changed
- Removed `no-forward-ref` codelyzer rule from `tslint-ng2.json`
- Changed `no-inferrable-types` from `false` to `[true, "ignore-params"]`
- Changed `trailing-comma` for `multiline` from `"never"` to `"always"`
- Changed `one-line` properties to `"check-catch", "check-finally", "check-else", "check-open-brace", "check-whitespace"`
- Changed `whitespace` options to `"check-branch", "check-decl", "check-operator", "check-module", "check-separator", "check-type", "check-preblock"`

## [v1.1.1] - 2017-03-17
### Fixed
- Support for codelyzer 3.x for `tslint-ng2.json`

## [v1.1.0] - 2017-02-28
### Changed
- Removed `no-magic-numbers` rule from `tslint-base.json`
- Removed `object-literal-sort-keys` rule from `tslint-base.json`
- Changed `max-file-line-count` rule from `500` to `600` lines

## [v1.0.1] - 2017-02-06
### Fixed
- Set correct type name for Bluebird promise (`Bluebird`) for `no-floating-promises` rule.

## [v1.0.0] - 2017-02-05
### Added
- Created initial versions of `tslint-base.json` and `tslint-ng2.json`.

[unreleased]: https://github.com/codeschool/cs-tslint-rules/compare/v5.0.0...HEAD
[v5.0.0]: https://github.com/codeschool/cs-tslint-rules/compare/v4.1.0...v5.0.0
[v4.1.0]: https://github.com/codeschool/cs-tslint-rules/compare/v4.0.0...v4.1.0
[v4.0.0]: https://github.com/codeschool/cs-tslint-rules/compare/v3.1.2...v4.0.0
[v3.1.2]: https://github.com/codeschool/cs-tslint-rules/compare/v3.1.1...v3.1.2
[v3.1.1]: https://github.com/codeschool/cs-tslint-rules/compare/v3.1.0...v3.1.1
[v3.1.0]: https://github.com/codeschool/cs-tslint-rules/compare/v3.0.1...v3.1.0
[v3.0.1]: https://github.com/codeschool/cs-tslint-rules/compare/v3.0.0...v3.0.1
[v3.0.0]: https://github.com/codeschool/cs-tslint-rules/compare/v2.0.0...v3.0.0
[v2.0.0]: https://github.com/codeschool/cs-tslint-rules/compare/v1.1.1...v2.0.0
[v1.1.1]: https://github.com/codeschool/cs-tslint-rules/compare/v1.1.0...v1.1.1
[v1.1.0]: https://github.com/codeschool/cs-tslint-rules/compare/v1.0.1...v1.1.0
[v1.0.1]: https://github.com/codeschool/cs-tslint-rules/compare/v1.0.0...v1.0.1
[v1.0.0]: https://github.com/codeschool/cs-tslint-rules/tree/v1.0.0
