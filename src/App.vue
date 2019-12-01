<template>
    <div class="main-container">
    <navigation/>
    <div id="app">
      <home/>
    </div>
  </div>
</template>
<script>
import Home from './views/Home.vue'
import Navigation from './views/Navigation.vue'

export default {
  components: {
    'home' : Home,
    'navigation' : Navigation
  }
}
</script>

<style lang="scss">
@import "scss/_basics.scss";

</style>
