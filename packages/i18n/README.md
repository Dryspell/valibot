# Valibot i18n

The official i18n translations for Valibot. See the [internationalization guide](https://valibot.dev/guides/internationalization/) for more details.

## Current status

| Language        | Pull Request       | Status |
| --------------- | ------------------ | ------ |
| Chinese (zh-CN) | [#419][pr-419-url] | ✅     |
| Chinese (zh-TW) | [#427][pr-427-url] | ✅     |
| English (en)    | [#397][pr-397-url] | ✅     |
| German (de)     | [#397][pr-397-url] | ✅     |
| French (fr)     | [#418][pr-418-url] | ✅     |
| Slovenian (sl)  | [#422][pr-422-url] | 🚧     |
| Ukrainian (uk)  | [#423][pr-423-url] | ✅     |

[pr-397-url]: https://github.com/fabian-hiller/valibot/pull/397
[pr-418-url]: https://github.com/fabian-hiller/valibot/pull/418
[pr-419-url]: https://github.com/fabian-hiller/valibot/pull/419
[pr-422-url]: https://github.com/fabian-hiller/valibot/pull/422
[pr-423-url]: https://github.com/fabian-hiller/valibot/pull/423
[pr-427-url]: https://github.com/fabian-hiller/valibot/pull/427

## Getting started

Step 1: Clone repository

```bash
git clone git@github.com:fabian-hiller/valibot.git
```

Step 2: Install dependencies

```bash
pnpm install
```

Step 3: Build core library

```bash
cd ./library && pnpm build
```

Step 4: Change to directory

```bash
cd ../packages/i18n
```

## Add language

1. Add ISO code to `src/types.ts` in line 4
2. Duplicate `src/en.ts` and change file name to ISO code
3. Change ISO code and translate messages in new file
4. Import new language file in `scripts/build.ts`
5. Add new import to `languages` array

## Build library

Execute build script

```bash
pnpm build
```