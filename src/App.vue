<template>
    <div class="main-container">
    <navigation/>
      <div id="app">
      

         <router-view/>

      </div>
  </div>
</template>
<script>
import Home from './views/Home.vue'
import Navigation from './views/Navigation.vue'
import Exercise from './views/Exercise.vue'




export default {
  components: {
    'home' : Home,
    'navigation' : Navigation
  }
}
</script>

<style lang="scss">
@import "scss/_basics.scss";
body {
  background-image: linear-gradient(rgba(40, 36, 37, 0.9) 100%, rgba(40, 36, 37, 0.7) 0%),
  url(./assets/background.jpg);
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
}

</style>
