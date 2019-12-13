<template>
  <div class="exercise">

    <exercises-list class="exercise-layout" />

    <exercise-detail />

    <rating />

  </div>
</template>

<script>

import ExercisesList from '@/components/ExercisesList.vue';
import ExerciseDetail from '@/components/ExerciseDetail.vue';
import Rating from '@/components/Rating.vue';


export default {
  name: 'exercise',
  components: {
    'exercises-list' : ExercisesList,
    'exercise-detail' : ExerciseDetail,
    'rating' : Rating,
  }
}
</script>


<style lang="scss" scoped>
@import "../scss/_basics.scss";

.exercise {
  display: flex;
}

.exercise-layout {
  flex: 0 0 30%;
}

</style>