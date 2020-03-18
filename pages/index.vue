<template>
  <div>
    <navbar/>
    <div class="main">
      <div>
        <carousel/>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from '../components/navbar'
import Carousel from '../components/carousel'

export default {
  name: 'Index',
  components: {
    Navbar,
    Carousel
  }
}
</script>

<style>
.main {
  width: 80rem;
  height: aotu;
  margin: 5rem auto;
}
</style>
