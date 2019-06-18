<template>
  <section class="menu">
    <div class="menu__banner"></div>
    <div class="menu__card">
      <button class="menu__card-button" v-on:click.stop="menuClick">Cold Dishes</button>
      <button class="menu__card-button" v-on:click.stop="menuClick">Style Dishes</button>
      <button class="menu__card-button" v-on:click="menuClick">Hot Dishes</button>
      <button class="menu__card-button" v-on:click="menuClick">Dumplings</button>
      <button class="menu__card-button" v-on:click="menuClick">Drinks</button>
    </div>
  </section>
</template>


<script>
import MenuCold from "@/components/MenuCold.vue";
import MenuDrinks from "@/components/MenuDrinks.vue";
import MenuDumplings from "@/components/MenuDumplings.vue";
import MenuHot from "@/components/MenuHot.vue";
import MenuStyleDish from "@/components/MenuStyleDish.vue";

  export default {
    data() {
      return {
        menu: ''
      }
    },
    methods: {
      menuClick: function(event) {
        //Run function to display correct menu for the button clicked
        this.menu = event.target.innerText;
      }
    },
    components: {
      MenuCold,
      MenuDrinks,
      MenuDumplings,
      MenuHot,
      MenuStyleDish
    }
  };
</script>

<style lang="scss">
.menu {
  &__banner {
    background-image: url("../assets/images/lantern2.jpeg");
    background-size: cover;
    background-position: center center;
    position: relative;
    height: 100vh;
  }

  &__card {
    width: 100vw;
    height: 100vh;
    background-color: $color-white; 
    display: flex;
    align-items: flex-start;
    justify-content: center;

    &-button {
      display: inline-block;
      padding: 0.46em 1.6em;
      border: 0.1em solid $color-black;
      margin: 1.6rem 0.8rem 1.5rem 0;
      border-radius: 0.12em;
      box-sizing: border-box;
      text-decoration: none;
      font-family: 'Roboto', sans-serif;
      font-weight: 300;
      font-size: 2rem;
      color: $color-black;
      text-align: center;
      transition: all 0.3s;

      &:hover {
        color: $color-white;
        background-color: $color-black;
      }
    }
  }
}

</style>