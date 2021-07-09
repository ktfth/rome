# `harness.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/compiler/lint/rules/harness.test.ts --update-snapshots` to update.

## `js/noAsyncPromiseExecutor`

### `0`

```

 lint/js/noAsyncPromiseExecutor/reject/1/file.ts:1:12 lint/js/noAsyncPromiseExecutor ━━━━━━━━━━━━━━━

  ✖ Promise executor functions should not be async.

    new Promise(async function foo() {})
                ^^^^^^^^^^^^^^^^^^^^^^^

  ℹ This can lead to lost errors and unnecessary indirection.


```

### `0: formatted`

```ts
new Promise(async function foo() {});

```

### `1`

```

 lint/js/noAsyncPromiseExecutor/reject/2/file.ts:1:12 lint/js/noAsyncPromiseExecutor ━━━━━━━━━━━━━━━

  ✖ Promise executor functions should not be async.

    new Promise(async () => {})
                ^^^^^^^^^^^^^^

  ℹ This can lead to lost errors and unnecessary indirection.


```

### `1: formatted`

```ts
new Promise(async () => {});

```

### `2`

```

 lint/js/noAsyncPromiseExecutor/reject/3/file.ts:1:16 lint/js/noAsyncPromiseExecutor ━━━━━━━━━━━━━━━

  ✖ Promise executor functions should not be async.

    new Promise(((((async () => {})))))
                    ^^^^^^^^^^^^^^

  ℹ This can lead to lost errors and unnecessary indirection.


```

### `2: formatted`

```ts
new Promise(async () => {});

```

### `3`

```

```

### `3: formatted`

```ts
new Promise(() => {});

```

### `4`

```

```

### `4: formatted`

```ts
new Promise(() => {}, async function unrelated() {});

```

### `5`

```

```

### `5: formatted`

```ts
class Foo {}
new Foo(async () => {});

```