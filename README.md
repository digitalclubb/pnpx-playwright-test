# pnpx-playwright-test
Issue using playwright-test with pnpx or as an installed dependency.

## pnpx

Trying to run:

```
pnpx folio --config=config.ts
```

Results in the following error:
> error: unknown option '--config=config.ts'

## Install dependency

Installing `folio` as a dependency:

```
pnpm add -D folio
```

Then running (via npm script):

```
folio --config=config.ts
```

Results in the same error:
> error: unknown option '--config=config.ts'

## npx

`playright-test` with `folio` only seems to work when `npx` is used:

```
npx folio --config=config.ts
```

> Running 1 test using 1 worker<br />
1 passed (1s)

