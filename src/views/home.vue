<template>
 <div>
   <!-- 头部组件 -->
   <Header/>
   <!-- 这是你的内容 -->
  <div class="home">
    <div>{{title}}</div>
    <!-- 跳转到登录 /login -->
    <RouterLink to="/login">login</RouterLink>
  </div>
 </div>
</template>

<script>
import { RouterLink } from 'vue-router'
// 引入header组件文件 header.vue
import Header from '@/components/header.vue'
export default {
  // 组件注册
  components: {
    Header
  },

  // 传值
  props: [],
  // data
  data () {
    return {
      title: 'home'
    }
  },
  // 生命周期 函数 ---start---
  // 详见 https://cn.vuejs.org/api/options-lifecycle.html#beforeunmount
  beforeCreate () {},
  created() {},
  beforeMount() {},
  mounted() {},
  beforeUpdate() {},
  updated() {},
  beforeUnmount() {},
  unmounted() {},
  // 生命周期 函数 ---start---

  // 计算属性
  computed: {},
  // 监听函数
  watch: {},
  // 过滤器
  filters: {},
  // 函数
  methods: {}
}
</script>

<style lang="scss" scoped>
@import "../assets/mixin.scss";
.home{
  width:100%;
  height: calc(100vh - 60px);
  @include flexCenter;
  flex-direction: column;
}
</style>
