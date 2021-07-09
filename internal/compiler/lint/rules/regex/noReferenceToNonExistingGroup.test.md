# `noReferenceToNonExistingGroup.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/compiler/lint/rules/regex/noReferenceToNonExistingGroup.test.ts --update-snapshots` to update.

## `Dangling backslash in regex`

### `0`

```

 lint/regex/noReferenceToNonExistingGroup/reject/1/file.ts:1:20
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 18 group.

    let foo = /([abc]+)=\18/;foo;
                        ^^^


```

### `0: formatted`

```ts
let foo = /([abc]+)=\18/;
foo;

```

### `1`

```

 lint/regex/noReferenceToNonExistingGroup/reject/2/file.ts:1:20
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 49 group.

    let foo = /([abc]+)=\49/;foo;
                        ^^^


```

### `1: formatted`

```ts
let foo = /([abc]+)=\49/;
foo;

```

### `2`

```

 lint/regex/noReferenceToNonExistingGroup/reject/3/file.ts:1:20
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 78 group.

    let foo = /([abc]+)=\78/;foo;
                        ^^^


```

### `2: formatted`

```ts
let foo = /([abc]+)=\78/;
foo;

```

### `3`

```

 lint/regex/noReferenceToNonExistingGroup/reject/4/file.ts:1:20
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 99 group.

    let foo = /([abc]+)=\99/;foo;
                        ^^^


```

### `3: formatted`

```ts
let foo = /([abc]+)=\99/;
foo;

```

### `4`

```

 lint/regex/noReferenceToNonExistingGroup/reject/5/file.ts:1:19
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 19 group.

    let foo = /(([abc])\19)+=\28/;foo;
                       ^^^

 lint/regex/noReferenceToNonExistingGroup/reject/5/file.ts:1:25
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 28 group.

    let foo = /(([abc])\19)+=\28/;foo;
                             ^^^


```

### `4: formatted`

```ts
let foo = /(([abc])\19)+=\28/;
foo;

```

### `5`

```

 lint/regex/noReferenceToNonExistingGroup/reject/6/file.ts:1:20
lint/regex/noReferenceToNonExistingGroup ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid nonexistent group names. Check the 19 group.

    let foo = /([abc]+)=\199/;foo;
                        ^^^


```

### `5: formatted`

```ts
let foo = /([abc]+)=\199/;
foo;

```

### `6`

```

```

### `6: formatted`

```ts
let foo = /([abc]+)=\u0001/;
foo;

```

### `7`

```

```

### `7: formatted`

```ts
let foo = /([abc]+)=\u0002/;
foo;

```

### `8`

```

```

### `8: formatted`

```ts
let foo = /([abc]+)=8/;
foo;

```

### `9`

```

```

### `9: formatted`

```ts
let foo = /([abc]+)=9/;
foo;

```

### `10`

```

```

### `10: formatted`

```ts
let foo = /([abc]+)=\t9/;
foo;

```

### `11`

```

```

### `11: formatted`

```ts
let foo = /([abc]+)=\u001b8/;
foo;

```

### `12`

```

```

### `12: formatted`

```ts
let foo = /([abc]+)=\u00ff/;
foo;

```

### `13`

```

```

### `13: formatted`

```ts
let foo = /([abc]+)=\?7/;
foo;

```