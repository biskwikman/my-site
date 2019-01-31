<template>
  <div class=Header>
    <nuxt-link to="/" style="text-decoration:none"><h1 class="HeaderTitle">{{ headerTitle }}</h1></nuxt-link>
    <p><nuxt-link class="lang" to="/" style="text-decoration:none">Eng</nuxt-link>/<nuxt-link class="lang" to="/jp/" style="text-decoration:none">日本語</nuxt-link></p>
    <div class="HeaderLinks">
      <a href="https://qiita.com/biskwikman"><img src="../static/qiita-rect.png" height="20px"></a>
      <a href="https://medium.com/@djosephhenri"><img src="../static/Monogram.svg" width="20px" height="20px"></a>
      <a href="https://github.com/biskwikman"><img src="../static/GitHub-Mark-120px-plus.png" width="20px" height="20px"></a>
      <a href="https://twitter.com/biskwikman"><img src="../static/twitter.png" width="20px" height="20px"></a>
    </div>
  </div>
</template>

<script>
  export default {
    data: function () {
      return {
        headerTitle: "Dan Henri"
      }
    }
  }
</script>

<style scoped>
.lang {
  color: #35495e;
}

.Header {
  display: flex;
  background-color: #e0e0e0;
  padding: 1vh 2vh;
  justify-content: space-between;
  align-items: center;
}

.HeaderLinks a {
  padding: 0px 5px;
}

.HeaderTitle {
  font-family: "Sawarabi Mincho", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  font-weight: 200;
  font-size: 5vh;
  color: #35495e;
  letter-spacing: 1px;
}
</style>