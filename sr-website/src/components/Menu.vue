<template>
  <section class="menu">
    <div class="menu__banner">
    <div class="menu__card">

      <button class="menu__card-button menu__card-button--cold" @click="menuClick">Cold Dishes</button>
      <button class="menu__card-button" @click="menuClick">Style Dishes</button>
      <button class="menu__card-button" @click="menuClick">Hot Dishes</button>
      <button class="menu__card-button" @click="menuClick">Dumplings</button>
      <button class="menu__card-button" @click="menuClick">Drinks</button>

        <div class="menu__dish">
            <component v-bind:is="menu"></component>
        </div>
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
        //Vue won't allow keyword 'style' to be used as component name
        if (menuText === 'style') {
          menuText = 'styled'
        }
        
        this.menu = menuText;
      }
    },
    components: {
      'cold': MenuCold,
      'drinks': MenuDrinks,
      'dumplings': MenuDumplings,
      'hot': MenuHot,
      'styled': MenuStyleDish
    }
  };
</script>

<style lang="scss">
.menu {
  &__banner {
    background: url("../assets/images/lantern2.jpeg") center/85% fixed;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  &__card {
    background-color: $color-white; 
    display: grid;
    grid-template-columns: 10em repeat(5, 1fr) 10em;
    grid-template-rows: 10em auto;
    grid-gap: 1.5em;
    justify-content: center;
    max-width: 70vw;
    min-height: 100vh;

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
      line-height: 1.4;
    }

    &-name {
      font-size: 1.8rem;
    }
  }
}

</style>