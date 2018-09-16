<template>
  <div>
    <app-header/>
    <div class="container">
      <div class="project-description">
        <h6 class="wording">
          <strong>jpn-atlas</strong> はNPMで公開されたツールです。ウェブのためにTopoJSONフォームで国、都道府県と地方公共団体の境界データを届いています。詳細については<strong><a href="https://www.npmjs.com/package/jpn-atlas">NPMページ</a></strong>か<strong><a href="https://github.com/biskwikman/jpn-atlas">Githubリポジトリ</a></strong>を見てください。または<strong><a href="https://unpkg.com/jpn-atlas/">UNPKG</a></strong>からデータを受け取れます。
        </h6>
      </div>
      <div class="link-pic">
        <div class ="thumbnail" style="background-image: url('https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/jpn-atlas.png')"></div>
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
  /*background-image: linear-gradient(#ffffff, #a7d0e8);*/
  background-color: white;
}

.container > * {
  margin: 10px;
}

.project-description {
  display: flex;
  justify-content: center;
  width: 400px;
  height: auto;
}

.link-pic {
  display: flex;
  width: 40vw;
  height: 85vh;
  margin-top: 8vh;
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
  line-height: 1.8;
  color: #526488;
  text-align: center;
  padding-top: 8vh;
}

a {
  color: #354668;
}
</style>