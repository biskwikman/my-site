<template>
  <div>
    <app-header/>
    <div class="bgcolor">
      <section class="container intro">
        <div>
          <h1 class="title">
            私はマップを作るのが好きな都市計画者です
          </h1>
          <h2 class="subtitle">
            下記のプロジェクトを見てください
          </h2>
          <i class="arrow down"></i>
        </div>
        </section>
      <section class="container projects">
        <nuxt-link to="./projects/jpn-atlas"><app-project id="prone"></app-project></nuxt-link>
        <nuxt-link to="./projects/"><app-project id="prtwo"></app-project></nuxt-link>
        <nuxt-link to="./projects/"><app-project id="prthree"></app-project></nuxt-link>
      </section>
      </div>
  </div>
</template>

<script>
import AppHeader from '~/components/Header.vue'
import AppProject from '~/components/Project.vue'
export default {
  components: {
    'app-project': AppProject,
    'app-header': AppHeader
  }
}
</script>

<style>
#prone .thumbnail {
  background-image: url('https://i.imgur.com/Xux6n6C.png');
  background-position: 50% 5%;
  background-size: 75vh 52.5vh;
  width: 100%;
  height: 100%;
}

#prtwo .thumbnail {
  background-image: url('https://i.imgur.com/grIkcJf.png');
  background-position:center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

#prthree .thumbnail {
  background-image: url('https://i.imgur.com/6rlc7E9.png');
  background-position:center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

.bgcolor {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background-image: linear-gradient(#ffffff, #a7d0e8);
}

.container.intro {
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.projects > * {
  padding: 15px;
}

.container.projects {
  min-height: 50vh;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Sawarabi Mincho", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.subtitle {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-weight: 200;
  font-size: 28px;
  color: #526488;
  word-spacing: 5px;
  padding: 20px;
}

i {
    border: solid black;
    border-width: 0 3px 3px 0;
    border-color: #526488;
    display: inline-block;
    padding: 20px;
}

.down {
    transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
}
</style>
