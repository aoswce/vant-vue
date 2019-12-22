<template>
  <div class="about">
    <h6>This is an about page</h6>
    <van-button type="default" to="create">种花</van-button>
    <van-button type="primary" to="web">主页</van-button>
    <van-uploader v-model="fileList" multiple />
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
