<template>
  <div class="hello">
    <h3>例:</h3>
    <paginate
      v-model="page"
      :page-count="20"
      :page-range="3"
      :margin-pages="2"
      :click-handler="clickCallback"
      :prev-text="'上一页'"
      :next-text="'下一页'"
      :container-class="'pagination'"
      :page-class="'page-item'"
      :page-link-class="'page-link'"
      :prev-class="'page-item'"
      :prev-link-class="'page-link'"
      :next-class="'page-item'"
      :next-link-class="'page-link'">
    </paginate>
    <h4>属性</h4>
    <table class="table table-sm text-left">
      <tr>
        <td width="150">page-count</td>
        <td>总页数(必须)</td>
      </tr>
      <tr>
        <td>page-range</td>
        <td>显示的页面范围。默认值：3</td>
      </tr>
      <tr>
        <td>margin-pages</td>
        <td>两边显示的页数</td>
      </tr>
      <tr>
        <td>click-handler</td>
        <td>翻页后回掉方法</td>
      </tr>
      <tr>
        <td>container-class</td>
        <td>最外层dom(ul)的类名</td>
      </tr>
      <tr>
        <td>page-class</td>
        <td>li的类名</td>
      </tr>
      <tr>
        <td>page-link-class</td>
        <td>a的类名</td>
      </tr>
      <tr>
        <td>prev-class</td>
        <td>上一页li的类名</td>
      </tr>
      <tr>
        <td>prev-link-class</td>
        <td>上一页a的类名</td>
      </tr>
      <tr>
        <td>next-class</td>
        <td>下一页li的类名</td>
      </tr>
      <tr>
        <td>next-link-class</td>
        <td>下一页a的类名</td>
      </tr>
      <tr>
        <td>break-view-class</td>
        <td>中间...li的类名</td>
      </tr>
      <tr>
        <td>break-view-link-class</td>
        <td>中间...a的类名</td>
      </tr>
      <tr>
        <td>active-class</td>
        <td>当前页li的选中状态类名,默认active</td>
      </tr>
      <tr>
        <td>disabled-class</td>
        <td>禁用的类名,默认disabled</td>
      </tr>
      <tr>
        <td>no-li-surround</td>
        <td>是否去掉li，只有a,自定义样式</td>
      </tr>
      <tr>
        <td>first-last-button</td>
        <td>是否显示首页和尾页,默认false</td>
      </tr>
      <tr>
        <td>first-button-text</td>
        <td>首页文本</td>
      </tr>
      <tr>
        <td>last-button-text</td>
        <td>尾页文本</td>
      </tr>
      <tr>
        <td>hide-prev-next</td>
        <td>是否隐藏上一页、下一页当到首页和尾页时,默认false</td>
      </tr>
    </table>
    <!-- bootstrap 分页dom
    <ul class="pagination">
      <li class="page-item"><a class="page-link" href="#">Previous</a></li>
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">3</a></li>
      <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>
    -->
  </div>
</template>

<script>
  import Paginate from 'vuejs-paginate'
  export default {
    name: 'HelloWorld',
    components: { Paginate },
    data () {
      return {
        page: 10  //绑定的页数（初始化的）
      }
    },
    methods: {
      clickCallback (pageNum) {
        console.log(pageNum)
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
