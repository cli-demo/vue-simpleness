<template>
  <div class="login">
   <div>{{title}}</div>
    <!-- 跳转到首页 /home -->
    <RouterLink to="/home">home</RouterLink>
  </div>
</template>

<script>
import { RouterLink } from 'vue-router'
export default {
  data() {
    return {
      title: 'login'
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/mixin.scss";
.login{
  width:100%;
  height: calc(100vh - 60px);
  @include flexCenter;
  flex-direction: column;
}
</style>
