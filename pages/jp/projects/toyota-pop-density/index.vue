<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          下は population density map of Toyota City, Japan. This was made mostly using the newline delimited JSON NPM tool, <a href="https://www.npmjs.com/package/ndjson-cli"><strong>ndjson-cli</strong></a>, in the command line. Which in its own way allow you to manipulate data in Javascript like you would in Python Pandas or R. To follow the process I used for this, check out my <a href="https://medium.com/@djosephhenri/creating-a-population-density-map-of-toyota-city-japan-using-d3-geos-cli-and-some-other-stuff-705632a55e8f"><strong>blog</strong></a>. I've recorded each step, except for the legend, which is just html and css.
        </h6>
      </div>
      <div class="link-pic">
        <div class ="thumbnail" style="background-image: url('https://biskwikman.github.io/projects/toyota-density-map/toyota-choumes-color.svg')"></div>
      </div>
      <div class="legend">
        <div class="legend-title">
          <p>People per Hectare (10000 square meters)</p>
        </div>
        <div class="symbols">
          <div class="color 1" style="background-color: #fff7ec"></div>
          <div class="color 2" style="background-color: #fee8c8"></div>
          <div class="color 3" style="background-color: #fdd49e"></div>
          <div class="color 4" style="background-color: #fdbb84"></div>
          <div class="color 5" style="background-color: #fc8d59"></div>
          <div class="color 6" style="background-color: #ef6548"></div>
          <div class="color 7" style="background-color: #d7301f"></div>
          <div class="color 8" style="background-color: #990000"></div>
        </div>
        <div class="description">
          <div class="text-container"><p class ="text 1">0 - 1</p></div>
          <div class="text-container"><p class ="text 2">1 - 2</p></div>
          <div class="text-container"><p class ="text 3">2 - 4</p></div>
          <div class="text-container"><p class ="text 4">4 - 10</p></div>
          <div class="text-container"><p class ="text 5">10- 30</p></div>
          <div class="text-container"><p class ="text 6">30 - 60</p></div>
          <div class="text-container"><p class ="text 7">60 - 120</p></div>
          <div class="text-container"><p class ="text 8">120 - 265</p></div>
        </div>
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
  height: auto;
  background-image: linear-gradient(#ffffff, #a7d0e8);
}

.project-description {
  display: flex;
  justify-content: center;
  width: 100vw;
  margin: 8vh;
}

.link-pic {
  display: flex;
  width: 100vw;
  height: 120vh;
}

.link-pic .thumbnail {
  background-position: center;
  background-size: auto;
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

.legend {
  display: flex;
  flex-wrap: wrap;
  margin-right: auto;
}

.legend-title {
  height: 15px;
  width: auto;
  margin: 10px;
  flex-basis: 100%;
}
.color {
  height: 15px;
  width: 15px;
  margin: 10px;
}

.text-container {
  height: 15px;
  width: auto;
  margin: 10px;
}

p {
  font-size: 100%;
}
</style>