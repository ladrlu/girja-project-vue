<template>
  <header>

    <nav>
      <div class="header">
        <div class="hamburger-box" @click='openMenu = !openMenu'>
          <div class="hamburger"></div>
        </div>
        <h1>Girja HardStyle Gym APP</h1>
      </div>


      <ul class="menu" v-bind:class="{'open' : openMenu}">
        <li><router-link to="/exercise">Cviky</router-link></li>
        <li><a href="">Nový trénink</a></li>
        <li><a href="">Historie</a></li>
        <li><a href="">Progress</a></li>
      </ul>
    </nav>

  </header>


</template>

<script>
  export default {
    data: function () {
      return {
        openMenu: false
      }
    },
    name: 'navigation',
  }
</script>

<style lang="scss" scoped>
  @import "../scss/_basics.scss";

  .header {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    @include media (md) {
      flex-wrap: nowrap;
    }
  }

  nav {
    margin: 0;
    padding: 1.5rem 1.5rem 1.5rem 1.5rem;
    margin: 0 0 1.5rem 0;
    background-color: $main-color-light;
    border-radius: 0 0 5px 5px;
  }

  .menu {
    list-style: none;
    margin: 3rem 0 1.5rem 0;
    padding: 0;
    display: none;

    li {
      background-color: rgba(255, 255, 255, 0.3);
      margin: 1rem 0;
      padding: 0.5rem 0.5rem 0.5rem 1.5rem;
      border-radius: 5px;
      &:hover,
      &:focus {
        background-color: $main-color;
      }
    }

    a {
      text-decoration: none;
      color: $base-black;
      font-weight: 700;
      font-size: 2rem;
      text-transform: uppercase;
    }

    &.open {
      display: block;
    }
  }

  .hamburger {
    display: block;
    height: 4px;
    width: 30px;
    background-color: $base-black;
    z-index: 99;

    &:before {
      content: '';
      display: block;
      height: 4px;
      width: 30px;
      background-color: $base-black;
      transform: translate(0, 7px);
    }

    &:after {
      content: '';
      display: block;
      height: 4px;
      width: 30px;
      background-color: $base-black;
      transform: translate(0, -11px);
    }

    &-box {
      cursor: pointer;
      padding: 0.5rem;
      width: 30px;
      margin: 0.5rem 0;
      order: 2;
      @include media(md) {
        order: 1;
      }
    }
  }
</style>