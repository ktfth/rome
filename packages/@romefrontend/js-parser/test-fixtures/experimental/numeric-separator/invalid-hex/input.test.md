# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romefrontend/js-parser/index.test.ts --update-snapshots` to update.

## `experimental > numeric-separator > invalid-hex`

### `ast`

```javascript
JSRoot {
	body: Array []
	comments: Array []
	corrupt: false
	diagnostics: Array []
	filename: "input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "input.js"
		end: Object {
			column: 0
			index: 9
			line: 2
		}
		start: Object {
			column: 0
			index: 0
			line: 1
		}
	}
	directives: Array [
		JSDirective {
			value: "\\x1_0"
			loc: Object {
				filename: "input.js"
				end: Object {
					column: 8
					index: 8
					line: 1
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
		}
	]
}
```

### `diagnostics`

```
✔ No known problems!

```