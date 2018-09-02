<template>
  <div>
    <app-header/>
      <section class="container intro">
        <div>
          <h1 class="title">
            I'm Dan. I'm an urban planner. I like to make maps.
          </h1>
          <h2 class="subtitle">
            Check out some of the things I'm working on below.
          </h2>
          <i class="arrow down"></i>
        </div>
      </section>
      <section class="container projects">
        <nuxt-link to="./projects/"><app-project/></nuxt-link>
        <nuxt-link to="./projects/"><app-project/></nuxt-link>
      </section>
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
.container.intro {
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.projects > * {
  padding: 20px;
}

.container.projects {
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
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

