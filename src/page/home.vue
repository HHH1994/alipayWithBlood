<style  lang="less" scoped>

</style>
<template>
    <div class="home">
      <tab>
        <tab-item selected @on-item-click="onItemClick">已发货</tab-item>
        <tab-item @on-item-click="onItemClick">未发货</tab-item>
      </tab>
    </div>
</template>
<script>
  import { Tab, TabItem, Sticky, Divider, XButton, Swiper, SwiperItem } from 'vux'

  export default {
    components: {
      Tab,
      TabItem,
      Sticky,
      Divider,
      XButton,
      Swiper,
      SwiperItem
    },
    data () {
      return {
        index: 0,
        getBarWidth: function (index) {
          return (index + 1) * 22 + 'px'
        }
      }
    },
    methods: {
      onItemClick (index) {

        console.log('on item click:', index)
      }
    }
  }
</script>
