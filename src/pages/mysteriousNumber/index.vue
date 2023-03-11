<template>
  <view class="content">神秘数字</view>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      toolsList: [{ text: '图片加 水印' }],
    }
  },
  created() {
    console.log('created')
  },
  onLoad() {
    console.log('onload')
  },
  methods: {},
})
</script>
