# bisheng-plugin-api-doc

[![npm package](https://img.shields.io/npm/v/bisheng-plugin-api-doc.svg?style=flat-square)](https://www.npmjs.org/package/bisheng-plugin-api-doc)
[![NPM downloads](http://img.shields.io/npm/dm/bisheng-plugin-api-doc.svg?style=flat-square)](https://npmjs.org/package/bisheng-plugin-api-doc)

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
