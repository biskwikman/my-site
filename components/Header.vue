<template>
  <div class=Header>
    <h1 class="HeaderTitle">{{ headerTitle }}</h1>
    <div class="HeaderLinks">
      <a href="https://medium.com/@djosephhenri"><img src="../static/Monogram.svg" width="20px" height="20px"></a>
      <a href="https://github.com/biskwikman"><img src="../static/GitHub-Mark-120px-plus.png" width="20px" height="20px" ></a>
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

<style>
.Header {
  display: flex;
  background-color: #f1f1f1;
  padding: 10px 10px;
  justify-content: space-between;
  align-items: center;
}

.HeaderLinks {
  /*float: right;*/
}

.HeaderLinks a {
  padding: 10px 10px;
}

.HeaderTitle {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  font-weight: 200;
  font-size: 40px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>