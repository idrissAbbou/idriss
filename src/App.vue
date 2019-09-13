<template>
  <div id="app">
    <app-nav @pageChanged="location = $event"></app-nav>
    <app-header v-if="location == 'home'"></app-header>
    <app-technologies v-if="location == 'technologies'"></app-technologies>
    <app-study v-if="location == 'study'"></app-study>
    <app-projects v-if="location == 'projects'"></app-projects>
  </div>
</template>

<script>
import Vue from 'vue';

import Header from "./components/header.vue";
import meNav from "./components/navbar.vue";
import Technologies from "./components/technologies.vue";
import Study from "./components/study.vue";
import Projects from "./components/projects.vue";

import BootstrapVue from 'bootstrap-vue';
Vue.use(BootstrapVue);
export default {
  data() {
    return {
      location: 'home'
    }
  },
  components: {
    appHeader: Header,
    appNav: meNav,
    appTechnologies: Technologies,
    appStudy: Study,
    appProjects: Projects
  }
}
</script>

<style lang="scss">
  @import 'node_modules/bootstrap/scss/bootstrap';
  @import 'node_modules/bootstrap-vue/src/index.scss';
  body {
    font-family: 'Montserrat', sans-serif;
  }
  .selector-for-some-widget {
    box-sizing: content-box !important;
  } 
</style>
