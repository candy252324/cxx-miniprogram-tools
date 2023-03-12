<template>
  <view class="tools-list p-16">
    <div v-for="item in list" @click="go(item.url)" class="tools-item-wrapper">
      <div class="tools-item flex-center border-radius-4">
        {{ item.text }}
      </div>
    </div>
  </view>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      list: [
        { text: '图片水印', url: '/pages/waterMarker/index' },
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

<style lang="scss">
.tools-list {
  .tools-item-wrapper {
    position: relative;
    width: 33.33%;
    height: 0;
    padding-bottom: 33.33%;
    display: inline-block;
    .tools-item {
      position: absolute;
      top: 0;
      left: 0;
      width: calc(100% - 16px);
      height: calc(100% - 16px);
      background: #678fbb;
      color: #fff;
    }
  }
}
</style>
