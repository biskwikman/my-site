<template>
  <div>
    <app-header/>
    <!--<div class="bgcolor">-->
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          <strong>jpn-atlas</strong> is a tool published through NPM which delivers ready to use boundary data for Japanese municipalities, prefectures, and the country itself. Published in TopoJSON for use on the web. For more info, check out the <strong><a href="https://www.npmjs.com/package/jpn-atlas">NPM page</a></strong>, <strong><a href="https://github.com/biskwikman/jpn-atlas">Github repo</a></strong>  or get the data directly from <strong><a href="https://unpkg.com/jpn-atlas/">UNPKG</a></strong>.
        </h6>
      </div>
      <div class="link-pic">
        <div class ="thumbnail" style="background-image: url('https://i.imgur.com/Xux6n6C.png')"></div>
      </div>
    </div>
    <!--</div>-->
  </div>
</template>

<script>

import AppHeader from '~/components/Header.vue'

export default {
  components: {
    'app-header': AppHeader
  }
}

</script>

<style scoped>

/*.bgcolor {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: center;
  background-image: linear-gradient(#d3efff, #83d0fc);
}*/

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start;
  min-height: 90.6vh;
  background-image: linear-gradient(#d3efff, #83d0fc);
}

.container > * {
  margin: 10px;
}

.project-description {
  display: flex;
  justify-content: center;
  width: 400px;
  height: 85vh;
}

.link-pic {
  display: flex;
  width: 500px;
  height: 85vh;
}

.link-pic .thumbnail {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

.wording {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: 200;
  font-size: 25px;
  color: #526488;
  word-spacing: 5px;
  line-height: 1.2;
  text-align: center;
  padding-top: 8vh;
}

a {
  color: #354668;
}
</style>