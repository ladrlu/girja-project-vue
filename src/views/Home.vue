<template>

        <div class="nav-box">

          <div class="nav-item-box">
              <router-link to="exercise" class="nav-item">
                  <h2>Cviky</h2>
                <img src="../assets/001-kettlebell.svg" alt="ikona kettlebellu">
              </router-link>
          </div>

          <div class="nav-item-box">
              <a href="" class="nav-item">
                <h2>Nový trénink</h2>
                <img src="../assets/002-add.svg" alt="ikona přidání tréninku">
              </a>
          </div>

          <div class="nav-item-box">
            <a href="" class="nav-item">
              <h2>Historie</h2>
              <img src="../assets/003-clock-circular-outline.svg" alt="ikona historie tréninku">
            </a>
          </div>

          <div class="nav-item-box">
            <a href="" class="nav-item">
              <h2>Progress</h2>
              <img src="../assets/line-chart.svg" alt="ikona historie tréninku">
            </a>
          </div>
           
        </div>

</template>

<script>


export default {
  name: 'home',
  components: {
    
  }
}
</script>

<style lang="scss" scoped>
@import "../scss/_basics.scss";
.nav-box {
    margin: 1.5rem -1.5rem 5rem -1.5rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;

}
.nav-item-box {
    flex: 0 1 100%;
    padding: 1.5rem;

    @include media (sm) {
        flex: 0 0 50%;
        max-width: auto;
    }
}
.nav-item {
    display: block;
    text-align: center;
    background-color: $main-color-light;
    padding: 2rem;
    border-radius: 5px;
    text-decoration: none;
    transition: 0.3s ease all;
    @include media (md) {
      padding: 3rem;
    }
    img {
      max-width: 10rem;
      @include media (md) {
        max-width: 15rem;
      }
       
    }
    h2 {
        color: $base-white;
    }
    &:hover,
    &:focus {
      background-color: $main-color;
    }
}

</style>
