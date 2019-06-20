<template>
  <section class="menu">
    <div class="menu__banner"></div>
    <div class="menu__card">

      <button class="menu__card-button menu__card-button--cold" @click="menuClick">Cold Dishes</button>
      <button class="menu__card-button" @click="menuClick">Style Dishes</button>
      <button class="menu__card-button" @click="menuClick">Hot Dishes</button>
      <button class="menu__card-button" @click="menuClick">Dumplings</button>
      <button class="menu__card-button" @click="menuClick">Drinks</button>

        <div class="menu__dish">
            <!-- <v-if="menu === cold" cold/>
            <v-if="menu === style" style/>
            <v-if="menu === hot" hot/>
            <v-if="menu === dumplings" dumplings/>
            <v-if="menu === drinks" drinks/> -->
            <component v-bind:is="menu"></component>
        </div>
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
        menu: 'cold'
      }
    },
    methods: {
      menuClick: function(event) {
        //Run function to display correct menu for the button clicked
        let menuText = event.target.innerText.toLowerCase();
        const space = menuText.indexOf(' ');
        if (space > 0) {
          menuText = menuText.slice(0, space);
        }
        
        this.menu = menuText;
      }
    },
    components: {
      'cold': MenuCold,
      'drinks': MenuDrinks,
      'dumplings': MenuDumplings,
      'hot': MenuHot,
      'style': MenuStyleDish
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
    // height: 100vh;
    background-color: $color-white; 
    display: grid;
    grid-template-columns: 10em repeat(5, 1fr) 10em;
    grid-template-rows: 10em auto;
    grid-gap: 1.5em;
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

      &--cold {
        grid-column-start: 2;
      }

      &:hover {
        color: $color-white;
        background-color: $color-black;
      }
    }
  }

  &__dish {
    grid-column-start: 2;
    grid-column-end: 7;
    font-size: 1.6rem;
    
    &-content {
      margin: 100px 0 5px 0;
    }

    &-name {
      font-size: 1.8rem;
    }
  }
}

</style>