<template>
  <div class="root">
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: Microsoft YaHei, Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: #323232;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

ul {
  list-style: none;
  padding: 0;
}

a,
a:link,
a:visited,
a:active,
a:hover {
  text-decoration: none;
  color: #999;
}

.clear-fix {
  zoom: 1;
}

.clear-fix:after {
  content: '';
  display: block;
  clear: both;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
