# vue_paginatron

vue 分页组件

### 配合bootstrap使用,效果更好
### Install the npm package.
npm install vuejs-paginate --save

## 使用demo

```
import Paginate from "vuejs-paginate";
<paginate
    v-model="page"                  //绑定当前页数
    :page-count="20"                //分页总数 必须项
    :page-range="3"
    :margin-pages="3"
    :click-handler="clickCallback"  //点击时的回调方法 使用点击的页码作为参数
    :prev-text="'上一页'"
    :next-text="'下一页'"
    :container-class="'pagination'"
    :page-class="'page-item'"
    :page-link-class="'page-link'"
    :prev-class="'page-item'"
    :prev-link-class="'page-link'"
    :next-class="'page-item'"
    :next-link-class="'page-link'"
    :first-last-button="true"       //是否开启首页和尾页
></paginate>
```

# Register the component.
## ES5
```
var Paginate = require('vuejs-paginate')
Vue.component('paginate', Paginate)
```

## ES6
```
import Paginate from 'vuejs-paginate'
Vue.component('paginate', Paginate)
```

## CDN

####use the latest release
`<script src="https://unpkg.com/vuejs-paginate@latest"></script>`

####or use the specify version
`<script src="https://unpkg.com/vuejs-paginate@0.9.0"></script>`

`Vue.component('paginate', VuejsPaginate)`



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
