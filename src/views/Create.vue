<template>
  <div class="about">
    <h6>爱种花</h6>
    <van-button type="default">默认按钮</van-button>
    <van-button type="primary">主要按钮</van-button>
    <van-uploader v-model="fileList" multiple/>
  </div>
</template>
<script>
import Vue from 'vue'
import { Button, Uploader } from 'vant'

Vue.use(Button, Uploader)

export default {
  name: 'about',
  components: {
    [Button.name]: Button,
    [Uploader.name]: Uploader
  },
  data () {
    return {
      fileList: [
        { url: 'https://img.yzcdn.cn/vant/leaf.jpg' }
      ]
    }
  },
  methods: {
    afterRead (file) {
      // eslint-disable-next-line no-console
      console.log(file)
    }
  }
}
</script>
