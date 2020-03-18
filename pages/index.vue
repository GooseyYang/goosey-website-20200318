<template>
  <div>
    <navbar/>
    <div class="container">
      <div class="clear-fix">
        <carousel/>
        <new-article-list/>
      </div>
    </div>
    <div class="main clear-fix">
      <div class="container">
        <left-list class="left__list"></left-list>
        <div class="right__list"></div>
      </div>
    </div>
    <div class="footer"></div>
  </div>
</template>

<script>
import Navbar from '../components/navbar'
import Carousel from '../components/carousel'
import newArticleList from '../components/newArticleList'
import LeftList from '../components/leftList'

export default {
  name: 'Index',
  components: {
    Navbar,
    Carousel,
    newArticleList,
    LeftList
  }
}
</script>

<style>
.container {
  width: 80rem;
  height: aotu;
  margin: 5rem auto 3rem auto;
}

.main {
  padding: 3rem 0;
  background-color: #efefef;
}

.main .container {
   width: 80rem;
  height: aotu;
  margin: 0 auto;
}

.left__list {
  float: left;
  width: 53.4375rem;
}

.right__list {
  float: right;
  width: 24.0625rem;
}

.footer {
  width: 100%;
  height: 3.125rem;
  line-height: 3.125rem;
  background: #6a4835;
}
</style>
