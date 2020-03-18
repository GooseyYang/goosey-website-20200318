<template>
  <div class="newArticleList">
    <ul class="article__cate clear-fix">
      <li class="article__cate__li active">全部</li>
      <li class="article__cate__li">前端</li>
      <li class="article__cate__li">设计</li>
      <li class="article__cate__li">后端</li>
    </ul>
    <ul class="new__article__list">
      <nuxt-link 
        to="/"
        class="new__artcle clear-fix"
        v-for="item in 6" 
        :key="item">
        <div class="new__article__cate">[类别]</div>
        <div 
          to="/"
          class="new__article__title"
          title="文章标题文章标">文章标题文章标题文章标题文章标题文章标题文章标题文章标题文章标题文章标题文章标题文章标题文章标题</div>
        <div class="new__article__date">2020-03-18</div>
      </nuxt-link>
    </ul>
    <div class="more__article">
      阅读更多
      <i class="el-icon-right"></i>
    </div>
  </div>
</template>
<script>
export default {
  name: 'newArticleList'
}
</script>
<style scoped>
.newArticleList {
  float: right;
  width: 40.625rem;
  height: 16.875rem;
  font-size: .875rem;
}

.article__cate__li {
  float: left;
  width: 6.125rem;
  height: 2rem;
  line-height: 2rem;
  vertical-align: middle;
  text-align: center;
  background: url('../assets/images/cate_bg.png') no-repeat;
  color: #6a4835;
}

.article__cate__li:hover,
.article__cate .active {
  background: url('../assets/images/cate_bg_active.png') no-repeat;
  color: #eee2cb;
}

.new__article__list {
  margin-top: .625rem;
}

.new__artcle {
  height: 1.875rem;
  line-height: 1.875rem;
  vertical-align: middle;
}

.new__article__cate {
  float: left;
  letter-spacing: 0.5rem;
}

.new__article__title {
  float: left;
  overflow: hidden;
  width: 28.125rem;
  height: 1.875rem;
  line-height: 1.875rem;
}

.new__article__date {
  float: right;
  font-size: .75rem;
}

.more__article {
  width: 6.875rem;
  height: 2.1875rem;
  line-height: 2.1875rem;
  vertical-align: middle;
  text-align: center;
  margin-left: 33.75rem;
  margin-top: .625rem;
  background-color: #6a4835;
  border-radius: .3125rem;
  color: #eee2cb;
}

.more__article:hover{
  cursor: pointer;
}
</style>