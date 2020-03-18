<template>
  <div class="navbar__bg">
    <div class="navbar__fg">
      <nuxt-link
        to="/" 
        class="logo"></nuxt-link>
      <ul class="navbar__list clear-fix">
        <nuxt-link
          to="/" 
          class="navbar__list__li active">首页</nuxt-link>
        <nuxt-link
          to="/article/list/1"
          class="navbar__list__li">一本正经鹅</nuxt-link >
        <nuxt-link
          to="/article/list/2"
          class="navbar__list__li">五彩缤纷鹅</nuxt-link >
        <nuxt-link
          to="/"
          class="navbar__list__li">关于鹅</nuxt-link >
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>
<style scoped>
  .navbar__bg {
    width: 100%;
    height: 3.75rem;
    border-top: .625rem solid #6a4835;
    background-color: #eee;
  }

  .navbar__fg {
    width: 80rem;
    height: 100%;
    margin: 0 auto;
  }

  .logo {
    display: inline-block;
    width: 3.75rem;
    height: 3.75rem;
    background: url('../assets/images/goose.jpg') no-repeat;
    background-size: 100%;
  }

  .navbar__list {
    float: right;
  }

  .navbar__list__li{
    float: left;
    width: 9.375rem;
    height: 3.125rem;
    line-height: 3.125rem;
    vertical-align: middle;
    text-align: center;
    border-radius: 0 0 5px 5px;
  }

  .navbar__list__li:hover,
   .navbar__list .active {
    background-color: #323232;
    color: #ffffff;
    cursor: pointer;
  }

</style>