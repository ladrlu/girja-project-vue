<template>
  <div>
      <h4>Hodnocení</h4>
      <image-rating src="@/assets/kettlebell-png.png"></image-rating>
  </div>
</template>

<script>

import {ImageRating} from 'vue-rate-it';

export default {
    components: {
        ImageRating
    }
}
</script>

<style lang="scss" scoped>
@import "../scss/_basics.scss";

</style>