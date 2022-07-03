---
layout: default
title: Home
nav_order: 1
description: "yuptoswagger.js is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# yuptoswagger.js 

[Get started now](#getting-started)
[View it on GitHub](https://github.com/yuptoswagger-js/yuptoswagger.js)

---

## Getting started
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

- <a href="#docs/configuration.md">[See configuration options]</a>

---

## About the project

yuptoswagger.js is &copy; 2022 by [Gjergj Kadriu](http://gjergjkadriu.com).

### License

yuptoswagger.js is distributed by an [MIT license](https://github.com/yuptoswagger-js/yuptoswagger.js/tree/main/LICENSE.txt).

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/yuptoswagger-js/yuptoswagger.js#contributing).

<!-- #### Thank you to the contributors of yuptoswagger.js!

<ul class="list-style-none">
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul> -->

### Code of Conduct

yuptoswagger.js is committed to fostering a welcoming community.

[View our Code of Conduct](https://github.com/yuptoswagger-js/yuptoswagger.js/tree/main/CODE_OF_CONDUCT.md) on our GitHub repository.
