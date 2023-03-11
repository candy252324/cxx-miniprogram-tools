<template>
  <view class="content">
    <div v-for="item in list" @click="go(item.url)">{{ item.text }}</div>
  </view>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      list: [
        { text: '图片加水印', url: '/pages/waterMarker/index' },
        { text: '神秘数字', url: '/pages/mysteriousNumber/index' },
      ],
    }
  },
  onLoad() {},
  methods: {
    go(url: string) {
      uni.navigateTo({ url })
    },
  },
})
</script>

<style></style>
