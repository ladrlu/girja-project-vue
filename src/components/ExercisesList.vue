<template>

  <div class="exercisesList">
    <div
     class="exercise"
     >
     <!-- v-for="(exercise,index) in list"
     v-bind:key="index"
     v-on:click="showDetail(index)" -->
     
        <h3>Název cviku</h3>
        
    </div>

    <div class="exercise"></div>

  </div>

</template>

<script>
export default {
    /* methods: {
        showDetail() {

        }
    } */
}
</script>


<style lang="scss" scoped>
@import "../scss/_basics.scss";

.exercise {
    display: block;
    text-align: center;
    background-color: $main-color-light;
    border-radius: 5px;
    margin-bottom: 1.5rem;
    text-decoration: none;
    transition: 0.3s ease all;
    @include media (md) {
      padding: 2rem;
    }
    h3 {
        color: $base-white;
        padding: 0.5rem; 
    }
    &:hover,
    &:focus {
      background-color: $main-color;
    }
}

</style>