<template>
  <nav class="fixed-top navbar navbar-expand-lg navbar-dark ">
      <transition name='fade'>
          <app-welcome v-if="welcome == true"  :welcome="welcome" v-on:welcomeColsed="welcome = $event"></app-welcome>
      </transition>
    <div class="container">
        <a class="navbar-brand" href="#" @click="showWelcome">AI</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item active" v-for="location in locations" :key="location" @click="pageChanged(location)" >
                    <a class="nav-link text-uppercase" href="#">{{location}}</a>
                </li>
            </ul>
        </div>
    </div>
  </nav>
</template>

<script>
import Welcome from "./welcome.vue";
export default {
    
    data() {
        return {
            locations: ['home', 'technologies', 'study', 'projects'],
            welcome: false
        }
    },
    methods: {
        pageChanged(val) {
            this.$emit('pageChanged', val);
        },
        showWelcome() {
            if(this.welcome == false) this.welcome = true;
            else this.welcome = false;
        }
    },
    components: {
        appWelcome: Welcome
    }
}
</script>

<style>
    nav {
        background-color: rgba(0,0,0, .2) !important;
    }
    @media (max-width: 992px) { 
        nav {
            background-color: rgba(0,0,0, 1) !important;
        }   
    }
</style>