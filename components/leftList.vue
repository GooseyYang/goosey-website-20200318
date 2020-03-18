<template>
  <div>
    <div class="list__title">一本正经 · 鹅</div>
    <div class="list__block clear-fix"
    v-for="item of 6"
    :key="item">
      <div class="article__img"></div>
      <div class="article__details">
        <nuxt-link 
          to="/"
          class="article__title">标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题</nuxt-link>
        <div class="article__date">发布日期：2020-03-09</div>
        <div class="line">
          <hr class="line--1">
          <hr class="line--2">
          <hr class="line--1">
        </div>
        <div class="article__text">正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文正文</div>
        <ul class="article__label">
          <li 
            class="article__label__li"
            v-for="item of 3"
            :key="item">标签</li>
        </ul>
      </div>
      <div class="active__line"></div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'LeftList'
}
</script>
<style scoped>
.list__title {
  padding-left: 1.25rem;
  border-left: .3125rem solid #6a4835;
  font-size: 1.25rem;
  color: #6a4835;
}

.list__block {
  position: relative;
  width: 100%;
  height: 9.375rem;
  padding-top: .625rem;
  margin-top: 1.25rem;
  background: #ffffff;
  border: .0625rem solid #ddd;
  border-radius: .3125rem;
}

.list__block:hover {
  cursor: pointer;
  border-color: #6a4835;
}

.list__block:hover .active__line{
  display: block;
}

.article__img {
  float: left;
  width: 13.4375rem;
  height: 7.8125rem;
  background-color: blanchedalmond;
}

.article__details {
  float: right;
  width: 38.125rem;
  height: 7.8125rem;
  margin-right: .9375rem;
  color: #6a4835;
}

.article__title {
  display: block;
  overflow: hidden;
  height: 2.1875rem;
  line-height: 2.1875rem;
}

.article__date {
  text-align: right;
  font-size: .75rem;
}

.article__text {
  overflow: hidden;
  height: 2rem;
  line-height: 1rem;
  font-size: .75rem;
  color: #999;
}

.article__label {
  margin-top: .625rem;
  font-size: .75rem;
}

.article__label__li {
  float: left;
  padding: 0 .5rem;
  margin: 0 .2rem;
  height: 1.125rem;
  background-color: black;
  border-radius: .3125rem;
  color: #eeeeee;
}

.line {
  margin-top: -0.5rem;
}

.line--1 {
  display: inline-block;
  width: .9375rem;
  height: .1875rem;
  background-color: #6a4835;
}

.line--2 {
  display: inline-block;
  width: 35.5rem;
  height: .0625rem;
  background-color: #6a4835;
}

.active__line {
  display: none;
  position: absolute;
  right: 0;
  top: 50%;
  margin-top: -1.5625rem;
  width: .3125rem;
  height: 3.125rem;
  background-color: #6a4835;
  border-radius: .3125rem 0 0 .3125rem;
}
</style>