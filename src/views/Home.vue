<template>

        <div class="nav-box">
        <div class="nav-item-box">
            <a href="" class="nav-item">
              <h2>Cviky</h2>
              <img src="../assets/001-kettlebell.svg" alt="ikona kettlebellu">
            </a>
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
    margin: 0 -1.5rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    @include media(md) {
        flex-wrap: nowrap;
    }
}
.nav-item-box {
    flex: 0 1 40rem;
    padding: 1.5rem;

    @include media (md) {
        flex: 1 1 33.3333%;
        max-width: auto;
    }
}
.nav-item {
    display: block;
    text-align: center;
    background-color: $main-color-light;
    padding: 5rem;
    border-radius: 5px;
    text-decoration: none;
    img {
        max-width: 15rem;
    }
    h2 {
        color: $base-white;
    }
}

</style>
