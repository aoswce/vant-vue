<template>
    <div>
      <h6>主页</h6>
      <van-button type="primary" to="create">我要花文</van-button>
    </div>
</template>

<script>
// 引入组件
import Vue from 'vue'
import { Button } from 'vant'
import 'vant/lib/button/style'
Vue.use(Button)
export default {
  name: 'web',
  comments: {
    [Button.name]: Button
  }
}
</script>
