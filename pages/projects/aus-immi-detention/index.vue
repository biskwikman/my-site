<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          This is a map showing every onshore immigration detention center in Australia and their population as of February 28th 2019. This does <em>not</em> include offshore immigration detention centers. This map was done completely in Python, using <a href="http://geopandas.org/"><strong>Geopandas</strong></a>, <a href="https://scitools.org.uk/cartopy/docs/latest/"><strong>Cartopy</strong></a>, <a href="https://matplotlib.org/"><strong>Matplotlib</strong></a>, and <a href="https://jupyterlab.readthedocs.io/en/stable/"><strong>Jupyter Lab</strong></a>. I originally made it in color, and then made the black and white version for the <a href="https://somethingaboutmaps.wordpress.com/2019/05/06/monochrome-mapping-competition/"><strong>Monochrome Mapping Competition</strong></a>, which I ended up liking better.
        </h6>
      </div>
      <div class="image-container">
        <div class="image">
          <img src="https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/aus-immi-detention-map-bw-en.png" alt="Onshore Immigration Detention Centers in Australia">
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
  font-family: "Quicksand", "Source Sans Pro", "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
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
