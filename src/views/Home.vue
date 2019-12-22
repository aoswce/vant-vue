<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div>
      <van-grid :border="true" :column-num="2">
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-1.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-2.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
        <van-grid-item>
          <van-image src="https://img.yzcdn.cn/vant/apple-3.jpg"/>
          <HelloWorld msg="Welcome to Your Vue.js App"/>
        </van-grid-item>
      </van-grid>

    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import Vue from 'vue'
import { Icon, Grid, GridItem, Image } from 'vant'
import HelloWorld from '@/components/HelloWorld.vue'

Vue.use(Icon, Grid, GridItem, Image)

export default {
  name: 'home',
  components: {
    HelloWorld,
    [Icon.name]: Icon,
    [Grid.name]: Grid,
    [GridItem.name]: GridItem,
    [Image.name]: Image
  }
}
</script>
