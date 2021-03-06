# CHANGELOG

## Introduction

This CHANGELOG tells you:

* when a release was made
* what is in each release

It also tells you what changes have been completed, and will be included in the next tagged release.

For each release, changes are grouped under these headings:

* _Backwards-Compatibility Breaks_: a list of any backwards-compatibility breaks
* _New_: a list of new features. If the feature came from a contributor via a PR, make sure you link to the PR and give them a mention here.
* _Fixes_: a list of bugs that have been fixed. If there's an issue for the bug, make sure you link to the GitHub issue here.
* _Dependencies_: a list of dependencies that have been added / updated / removed.
* _Tools_: a list of bundled tools that have been added / updated / removed.

## develop branch

The following changes have been completed, and will be included in the next tagged release.

## v0.0.3

Released Friday, 17th April 2020.

### Dependencies

* Removed unused dependency on `@ganbarodigital/ts-lib-error-reporting`
* Upgraded to latest `@ganbarodigital/ts-lib-base-n`
* Upgraded to latest `@ganbarodigital/ts-lib-uuid-parser`

## v0.0.2

Released Monday, 6th April 2020.

### Dependencies

* Upgraded everything to resolve a vulnerability in `minimist`
* Moved TypeScript et al into the `devDependencies` section

## v0.0.1

Released Thursday, 27th February 2020.

### New

* Added `uuidToBase32Url()`
* Added `uuidToBase36Url()`
* Added `uuidToBase64Url()`

### Fixes

### Dependencies

* Added deps:
  - `@ganbarodigital/ts-lib-base-n`
  - `@ganbarodigital/ts-lib-uuid-parser`
