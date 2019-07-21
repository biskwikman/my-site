<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          下は2019年02月19日のオーストラリア本土の移民収容センター人口の地図。沖合いにある移民収容センターが含まれません。この地図はPythonの<a href="http://geopandas.org/"><strong>Geopandas</strong></a>、<a href="https://scitools.org.uk/cartopy/docs/latest/"><strong>Cartopy</strong></a>、<a href="https://matplotlib.org/"><strong>Matplotlib</strong></a>、とJupyter Labで全部作られました。僕はこれを<a href="https://somethingaboutmaps.wordpress.com/2019/05/06/monochrome-mapping-competition/"><strong>Monochrome Mapping Competition</strong></a>に提出しました。
        </h6>
      </div>
      <div class="image-container">
        <div class="image">
          <img src="https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/aus-immi-detention-map-bw-jp.png" alt="Onshore Immigration Detention Centers in Australia">
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
  background-color: white;
}

.project-description {
  display: flex;
  justify-content: center;
  width: 100vw;
  margin: 8vh;
}

.image-container {
  display: flex;
  flex-direction: column;
  width: auto;
  height:auto;
}

.image {
  width: 100%;
  height: auto;
}

img {
  max-width: 100%;
  margin: 5vh;
}

.wording {
  font-family: "Quicksand", "Source Sans Pro", sans-serif;
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

p {
  font-size: 100%;
}
</style>
