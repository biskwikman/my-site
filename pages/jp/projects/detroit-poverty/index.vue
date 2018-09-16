<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          下のインタラクティブマップは<a href="http://www.detroitmi.gov/"><strong>デトロイト市</strong></a>の貧困率が表示されています。Python <a href="http://geopandas.org/"><strong>GeoPandas</strong></a>でデータが処理されて、<a href="https://www.mapbox.com/mapbox-gl-js/api/"><strong>Mapbox-gl.js</strong></a>で表示されています。このマップについてもっと詳しい作り方に興味があったら僕の<a href="https://medium.com/@djosephhenri/mapping-detroits-high-poverty-areas-and-their-access-to-public-transit-using-geopandas-mapbox-72fa21a0bd79"><strong>ブログ</strong></a>を見てください。
        </h6>
      </div>
      <div class="link-pic">
        <iframe src="https://biskwikman.github.io/projects/detroit-poverty-map/"></iframe>
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
  /*background-image: linear-gradient(#ffffff, #a7d0e8);*/
  background-color: white;
}

.project-description {
  display: flex;
  justify-content: center;
  width: 100vw;
  margin: 8vh;
}

.link-pic {
  display: flex;
  width: auto;
  height:auto;
}

iframe {
  width: 90vw;
  height: 90vh;
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