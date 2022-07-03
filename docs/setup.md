---
layout: default
title: Setup
nav_order: 2
---

# Setup
{: .no_toc }

{: .no_toc .text-delta }
## Getting started

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---
<!-- 
### Dependencies

yuptoswagger.js is built for [Jekyll](https://jekyllrb.com), a static site generator. View the [quick start guide](https://jekyllrb.com/docs/) for more information. yuptoswagger.js requires no special plugins and can run on GitHub Pages' standard Jekyll compiler. The [Jekyll SEO Tag plugin](https://github.com/jekyll/jekyll-seo-tag) is included by default (no need to run any special installation) to inject SEO and open graph metadata on docs pages. For information on how to configure SEO and open graph metadata visit the [Jekyll SEO Tag usage guide](https://jekyll.github.io/jekyll-seo-tag/usage/). -->

### Quick start: Using npm

```shell
$ npm install yuptoswagger.js
```
### Quick start: Using yarn

```shell
$ yarn add yuptoswagger.js
```

### yuptoswagger.js in action

```js
import * as yup from "yup";
import Compiler from "yuptoswagger.js";

// Initialize compiler
const options = {
  debug: true
}
const compiler = new Compiler(options);

const schema = yup.object().shape({
  first_name: yup.string().min(2).required(),
  last_name: yup.string().min(2).required(),
  email: yup.string().email().required(),
  password: yup.string().min(8).required(),
})
const swagger = compiler.compile(schema);
```
## Output:
```js
{
  type: 'object',
  fields: [
    { type: 'string', enum: [], minLength: 2 },
    { type: 'string', enum: [], minLength: 2 },
    { type: 'string', enum: [], format: 'email' },
    { type: 'string', enum: [], minLength: 8 }
  ]
}
```

### Configure yuptoswagger.js
- [See configuration options]({% link docs/configuration.md %})

<!-- View this site's [\_config.yml](https://github.com/yuptoswagger-js/yuptoswagger.js/tree/main/_config.yml) file as an example. -->
