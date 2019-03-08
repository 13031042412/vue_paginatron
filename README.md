# vue_paginatron

> vue 分页组件
# 配合bootstrap使用
# Install the npm package.
npm install vuejs-paginate --save

# Register the component.
# ES5
var Paginate = require('vuejs-paginate')
Vue.component('paginate', Paginate)
# ES6
import Paginate from 'vuejs-paginate'
Vue.component('paginate', Paginate)

# CDN
<!-- use the latest release -->
<script src="https://unpkg.com/vuejs-paginate@latest"></script>
<!-- or use the specify version -->
<script src="https://unpkg.com/vuejs-paginate@0.9.0"></script>
Vue.component('paginate', VuejsPaginate)



## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
