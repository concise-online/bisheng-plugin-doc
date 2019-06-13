# bisheng-plugin-api-doc

To extract api doc from Markdown.

## Usage

Install:

```bash
npm i --save bisheng-plugin-api-doc
```

Add 'bisheng-plugin-api-doc' to `bisehng.config.js`'s plugins.

```js
module.exports = {
  plugins: ['bisheng-plugin-api-doc'],
};
```

In Markdown:

```markdown
---
title: ...
...
---

This is description.

---

## API

This is api doc content.
```

In template:

```jsx
<div>
  { utils.toReactComponent(pageData.api) }
</div>
```

## Liscense

MIT
