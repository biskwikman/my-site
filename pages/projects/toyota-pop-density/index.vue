<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          Below is a population density map of Toyota City, Japan. This was made mostly using the newline delimited JSON NPM tool, <a href="https://www.npmjs.com/package/ndjson-cli"><strong>ndjson-cli</strong></a>, in the command line. Which in its own way allow you to manipulate data in Javascript like you would in Python Pandas or R. To follow the process I used for this, check out my <a href="https://medium.com/@djosephhenri/creating-a-population-density-map-of-toyota-city-japan-using-d3-geos-cli-and-some-other-stuff-705632a55e8f"><strong>blog</strong></a>. I've recorded each step, except for the legend, which is just html and css.
        </h6>
      </div>
      <div class="link-pic">
        <div class ="thumbnail" style="background-image: url('https://i.imgur.com/grIkcJf.png')"></div>
      </div>
    </div>
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

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: flex-start;
  min-height: 90.6vh;
  background-image: linear-gradient(#ffffff, #a7d0e8);
}

.container > * {
  margin: 40px;
}

.project-description {
  display: flex;
  justify-content: center;
  width: 100vw;
}

.link-pic {
  display: flex;
  width: 100vw;
  height: 100vh;
}

.link-pic .thumbnail {
  background-position: center;
  background-size: auto 100%;
  background-repeat: no-repeat;
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