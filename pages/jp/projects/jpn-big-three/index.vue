<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          下は日本の主要都市の人口密度地図。この地図を作るようにpythonで地図を表すことを学んだ。用いた用具は <a href="https://jupyterlab.readthedocs.io/en/stable/index.html"><strong>jupyterlab</strong></a>, <a href="http://geopandas.org/"><strong>geopandas</strong></a>, <a href="https://matplotlib.org/"><strong>matplotlib</strong></a> 及びに他の用具。pythonは楽しいと思う。今、<a href="https://pysal.readthedocs.io/en/latest/"><strong>pysal 2.0</strong></a>は出たからもっと良い地図キャプションをできる。もし地図の作り方は興味があれば<a href="https://qiita.com/biskwikman/items/b09de2b470e1dabcaed2"><strong>ここ</strong></a>でそれを書いた。
        </h6>
      </div>
      <div class="image-container">
        <div class="image">
          <img src="https://bit.ly/2YQep5D" alt="Population Density of Metropolitan Tokyo">
        </div>
        <div class="image">
          <img src="https://bit.ly/2OXehMX" alt="Population Density of Nagoya">
        </div>
        <div class="image">
          <img src="https://bit.ly/2KcwJT6" alt="Population Density of Osaka">
        </div>
        <div class="image">
          <img src="https://bit.ly/2CZhpTM" alt="Population Density of Tokyo 23 Wards">
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
  /*background-image: linear-gradient(#ffffff, #a7d0e8);*/
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