<template>
  <div class="exercise">
      <h2>Název cviku</h2>

      <img src="../assets/Podklad_pro_cviky.jpg" alt=""> 

    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea dolore numquam possimus sapiente error incidunt eligendi eius rem, alias ex adipisci. Soluta ipsum impedit a. Delectus autem, blanditiis consequuntur corporis minima fugiat, animi sit asperiores suscipit voluptatum necessitatibus itaque, exercitationem laborum hic impedit minus aliquam architecto aperiam optio iusto nulla. Pariatur nulla exercitationem quod, tempora error repellat beatae voluptas officiis, ratione modi voluptatem itaque cumque ab sequi corporis placeat unde ducimus rerum debitis eaque! Ullam, consectetur libero molestias provident aliquam quia at corporis debitis eius! A, quia vel. Cumque tempore pariatur deserunt in ratione impedit velit facilis soluta odit laborum!</p>

  </div>
</template>

<script>
export default {
  name: 'exercise',
  components: {
    
  }
}
</script>


<style lang="scss" scoped>
@import "../scss/_basics.scss";

.exercise {
    text-align: center;
    background-color: $main-color-light;
    padding: 2rem;
    border-radius: 5px;
    text-decoration: none;
    transition: 0.3s ease all;
    @include media (md) {
      padding: 3rem;
    }
    h2 {
        color: $base-white;
    }
    img {
      max-width: 30rem;
      @include media (sm) {
        max-width: 45rem;
      }
      @include media (md) {
        max-width: 60rem;
      } 
    }
    p {
        padding: 2rem;
        @include media (md) {
      padding: 3rem;
    }
    }
    
    
}

</style>