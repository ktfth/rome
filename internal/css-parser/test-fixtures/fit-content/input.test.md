# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/css-parser/index.test.ts --update-snapshots` to update.

## `fit-content`

```javascript
CSSRoot {
	body: [
		CSSRule {
			prelude: [
				CSSSelector {
					patterns: [
						CSSClassSelector {
							value: "style"
							loc: SourceLocation fit-content/input.css 1:0-1:6
						}
					]
					loc: SourceLocation fit-content/input.css 1:0-1:7
				}
			]
			block: CSSBlock {
				value: [
					CSSDeclaration {
						name: "grid-template-columns"
						value: [
							CSSFitContent {
								name: "fit-content"
								params: [
									CSSDimension {
										value: 8
										unit: "ch"
										loc: SourceLocation fit-content/input.css 2:36-2:39
									}
								]
								loc: SourceLocation fit-content/input.css 2:36-2:39
							}
							CSSFitContent {
								name: "fit-content"
								params: [
									CSSDimension {
										value: 8
										unit: "ch"
										loc: SourceLocation fit-content/input.css 2:53-2:56
									}
								]
								loc: SourceLocation fit-content/input.css 2:53-2:56
							}
							CSSDimension {
								value: 1
								unit: "fr"
								loc: SourceLocation fit-content/input.css 2:58-2:61
							}
						]
						important: false
						loc: SourceLocation fit-content/input.css 2:1-2:61
					}
				]
				startingTokenValue: "{"
				loc: SourceLocation fit-content/input.css 1:7-3:1
			}
			loc: SourceLocation fit-content/input.css 1:0-3:1
		}
		CSSRule {
			prelude: [
				CSSSelector {
					patterns: [
						CSSClassSelector {
							value: "style"
							loc: SourceLocation fit-content/input.css 5:0-5:6
						}
					]
					loc: SourceLocation fit-content/input.css 5:0-5:7
				}
			]
			block: CSSBlock {
				value: [
					CSSDeclaration {
						name: "width"
						value: [
							CSSIdentifier {
								value: "fit-content"
								loc: SourceLocation fit-content/input.css 6:8-6:19
							}
						]
						important: false
						loc: SourceLocation fit-content/input.css 6:1-6:19
					}
				]
				startingTokenValue: "{"
				loc: SourceLocation fit-content/input.css 5:7-7:1
			}
			loc: SourceLocation fit-content/input.css 5:0-7:1
		}
	]
	comments: []
	corrupt: false
	diagnostics: []
	path: RelativePath<fit-content/input.css>
	loc: SourceLocation fit-content/input.css 1:0-7:1
}
```