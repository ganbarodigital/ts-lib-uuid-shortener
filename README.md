# UUID Shortener for Typescript

## Introduction

This TypeScript library will shorten any [RFC 4122 UUID](http://www.ietf.org/rfc/rfc4122.txt) in a URL-friendly way.

- [Introduction](#introduction)
- [Quick Start](#quick-start)
- [V1 API](#v1-api)
  - [uuidToBase64Url()](#uuidtobase64url)
- [NPM Scripts](#npm-scripts)
  - [npm run clean](#npm-run-clean)
  - [npm run build](#npm-run-build)
  - [npm run test](#npm-run-test)
  - [npm run cover](#npm-run-cover)

## Quick Start

```
# run this from your Terminal
npm install @ganbarodigital/ts-lib-uuid-shortener
```

```typescript
// add this import to your Typescript code
import { uuidToBase64Url } from "@ganbarodigital/ts-lib-uuid-shortener/lib/v1"
```

__VS Code users:__ once you've added a single import anywhere in your project, you'll then be able to auto-import anything else that this library exports.

## V1 API

### uuidToBase64Url()

```typescript
import { Uuid } from "@ganbarodigital/ts-lib-uuid-parser/lib/v1";
import { uuidToBase64Url } from "@ganbarodigital/ts-lib-uuid-shortener/lib/v1"

export function uuidToBase64Url(uuid: Uuid): string;
```

`uuidToBase64Url()` is a _data transform_. It converts a `Uuid` into a base64url-encoded string.

For example:

```typescript
import { uuidFromFormatted } from "@ganbarodigital/ts-lib-uuid-parser/lib/v1";
import { uuidToBase64Url } from "@ganbarodigital/ts-lib-uuid-shortener/lib/v1"

const uuid = uuidFromFormatted("a968f2c6-b61b-4f88-a0e0-ec370a981a2e");
const shortened = uuidToBase64Url(inputValue);
console.log(shortened);
// outputs "qWjyxrYbT4ig4Ow3CpgaLg";
```

## NPM Scripts

### npm run clean

Use `npm run clean` to delete all of the compiled code.

### npm run build

Use `npm run build` to compile the Typescript into plain Javascript. The compiled code is placed into the `lib/` folder.

`npm run build` does not compile the unit test code.

### npm run test

Use `npm run test` to compile and run the unit tests. The compiled code is placed into the `lib/` folder.

### npm run cover

Use `npm run cover` to compile the unit tests, run them, and see code coverage metrics.

Metrics are written to the terminal, and are also published as HTML into the `coverage/` folder.