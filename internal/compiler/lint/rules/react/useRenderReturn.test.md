# `harness.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/compiler/lint/rules/harness.test.ts --update-snapshots` to update.

## `react/useRenderReturn`

### `0`

```

 lint/react/useRenderReturn/reject/1/file.tsx:3:10 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React from 'react';
    2 │ class Foo extends React.Component {
  > 3 │   render() {}
      │            ^^
    4 │ }


```

### `0: formatted`

```tsx
import React from "react";
class Foo extends React.Component {
	render() {}
}

```

### `1`

```

 lint/react/useRenderReturn/reject/2/file.tsx:3:10 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React from 'react';
    2 │ class Foo extends React.Component {
  > 3 │   render() {
      │            ^
  > 4 │     [1, 2, 3].map((num) => {
  > 5 │       return <div> Foo </div>
  > 6 │     });
  > 7 │   }
      │ ^^^
    8 │ }


```

### `1: formatted`

```tsx
import React from "react";
class Foo extends React.Component {
	render() {
		[1, 2, 3].map((num) => {
			return <div>
				 Foo 
			</div>;
		});
	}
}

```

### `2`

```

 lint/react/useRenderReturn/reject/3/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React from 'react';
    2 │ class Foo extends React.Component {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `2: formatted`

```tsx
import React from "react";
class Foo extends React.Component {
	render = () => {};
}

```

### `3`

```

 lint/react/useRenderReturn/reject/4/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React, {Component} from 'react';
    2 │ class Foo extends Component {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `3: formatted`

```tsx
import React, {Component} from "react";
class Foo extends Component {
	render = () => {};
}

```

### `4`

```

 lint/react/useRenderReturn/reject/5/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React from 'react';
    2 │ const Foo = class extends React.Component {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `4: formatted`

```tsx
import React from "react";
const Foo = class extends React.Component {
	render = () => {};
};

```

### `5`

```

 lint/react/useRenderReturn/reject/6/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React, {Component} from 'react';
    2 │ const Foo = class extends Component {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `5: formatted`

```tsx
import React, {Component} from "react";
const Foo = class extends Component {
	render = () => {};
};

```

### `6`

```

 lint/react/useRenderReturn/reject/7/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React from 'react';
    2 │ const Foo = class extends React.PureComponent {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `6: formatted`

```tsx
import React from "react";
const Foo = class extends React.PureComponent {
	render = () => {};
};

```

### `7`

```

 lint/react/useRenderReturn/reject/8/file.tsx:3:16 lint/react/useRenderReturn ━━━━━━━━━━━━━━━━━━━━━━

  ✖ The render method on a component must return content.

    1 │ import React, {PureComponent} from 'react';
    2 │ const Foo = class extends PureComponent {
  > 3 │   render = () => { }
      │                  ^^^
    4 │ }


```

### `7: formatted`

```tsx
import React, {PureComponent} from "react";
const Foo = class extends PureComponent {
	render = () => {};
};

```

### `8`

```

```

### `8: formatted`

```tsx
import React from "react";
class Foo extends React.Component {
	render() {
		return <div>
			Foo
		</div>;
	}
}

```

### `9`

```

```

### `9: formatted`

```tsx
import React from "react";
class Foo extends React.Component {
	render() {
		if (foo) {
			return <div>
				Foo
			</div>;
		} else {
			return void 0;
		}
	}
}

```

### `10`

```

```

### `10: formatted`

```tsx
class Foo {
	render = () => {
		return <></>;
	};
}

```

### `11`

```

```

### `11: formatted`

```tsx
class Foo {
	render = () => <></>;
}

```

### `12`

```

```

### `12: formatted`

```tsx
class Foo extends Bar {
	render() {}
}

```