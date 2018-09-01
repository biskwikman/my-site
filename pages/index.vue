<template>
  <div>
    <app-header/>
      <section class="container">
        <div>
          <!--<app-logo/>-->
          <h2 class="subtitle">
            I'm Dan. I'm an urban planner. I like to make maps.
          </h2>
        </div>
        <nuxt-link to="./projects/jpn.atlas.vue"><app-project/></nuxt-link>
      </section>
  </div>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import AppHeader from '~/components/Header.vue'
import AppProject from '~/components/Project.vue'
export default {
  components: {
    'app-project': AppProject,
    'app-header': AppHeader ,
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
</style>

