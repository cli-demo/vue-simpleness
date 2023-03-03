<template>
  <div class="header">
    <div class="header-title">这是一个组件：头部组件</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: 'header'
    }
  }
}
</script>

<style lang="scss" scoped>
// 目前主流css预处理语言有两种，分别是
// scss and less
// 这里没有使用less，使用的scss

// 定义了一个mixin 这样可以在每个页面都可以使用 ---start---
@import '../assets/mixin';
// 定义了一个mixin 这样可以在每个页面都可以使用 ---end---
.header{
  height:60px;
  background:#eee;
  &-title{ // 这种简写方式 ---> header-title
    color:#666;
    font-size: 20px;
    @include wh(100%, 100%);
    @include flexCenter;
  }
}
</style>
