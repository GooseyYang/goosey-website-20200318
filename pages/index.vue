<template>
  <div>
    <navbar/>
    <div class="main">
      <div class="clear-fix">
        <carousel/>
        <new-article-list/>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from '../components/navbar'
import Carousel from '../components/carousel'
import newArticleList from '../components/newArticleList'

export default {
  name: 'Index',
  components: {
    Navbar,
    Carousel,
    newArticleList
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
