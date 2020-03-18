<template>
  <el-carousel class="carousel">
    <el-carousel-item v-for="item in 1" :key="item">
      <nuxt-link 
        to="/"
        class="small">{{ item }}</nuxt-link>
    </el-carousel-item>
  </el-carousel>
</template>
<script>
export default {
  name: 'Carousel'
}
</script>
<style scoped>
.carousel {
  display: inline-block;
  width: 38.125rem;
  height: 16.875rem;
}

.el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
}

</style>