<template>
  <div>
    <app-header/>
    <div class="bgcolor">
      <section class="container intro">
        <div>
          <h1 class="title">
            I make maps, apps, and other tools using spatial data.
          </h1>
          <h2 class="subtitle">
            Check out some of the things I'm working on below.
          </h2>
          <i class="arrow down"></i>
        </div>
        </section>
      <section class="container projects">
        <nuxt-link to="./projects/jpn-atlas"><app-project id="prone"></app-project></nuxt-link>
        <nuxt-link to="./projects/toyota-pop-density"><app-project id="prtwo"></app-project></nuxt-link>
        <nuxt-link to="./projects/detroit-poverty"><app-project id="prthree"></app-project></nuxt-link>
        <a href="https://biskwikman.github.io/projects/jpn-noncitizen/"><app-project id="prfour"></app-project></a>
        <nuxt-link to="./projects/jpn-big-three"><app-project id="prfive"></app-project></nuxt-link>
        <nuxt-link to="./projects/aus-immi-detention"><app-project id="prsix"></app-project></nuxt-link>
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
  background-image: url('https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/jpn-atlas.png');
  background-position: 50% 5%;
  background-size: 75vh 52.5vh;
  width: 100%;
  height: 100%;
}

#prtwo .thumbnail {
  background-image: url('https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/toyota-dens.png');
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

#prthree .thumbnail {
  background-image: url('https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/detroit-pov.png');
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

#prfour .thumbnail {
  background-image: url('https://github.com/biskwikman/jpn-non-citizen-map/raw/master/images/noncitizen-image.png');
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}

#prfive .thumbnail {
  background-image: url('https://live.staticflickr.com/7812/46638480575_1d3b6d2995_b.jpg');
  background-position: 50% 35%;
  background-size: 230%;
  width: 100%;
  height: 100%;
}

#prsix .thumbnail {
  background-image: url('https://raw.githubusercontent.com/biskwikman/my-cdn/master/my-site/aus-immi-detention-map-bw-en.png');
  background-position: center;
  background-size: 120%;
  width: 100%;
  height: 100%;
}

.bgcolor {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  /*background-image: linear-gradient(#ffffff, #a7d0e8);*/
  background-color: white;
}

.container.intro {
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
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
  font-family: "Quicksand", "Source Sans Pro", sans-serif, -apple-system;
  font-weight: 300;
  font-size: calc(1em + 1.5vw);
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.subtitle {
  font-family: "Quicksand", "Source Sans Pro", sans-serif, -apple-system;
  font-weight: 200;
  font-size: calc(0.8em +1.2vw);
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
