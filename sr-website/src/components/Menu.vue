<template>
  <section class="menu">
    <div class="menu__banner"></div>
    <div class="menu__card">
      <button class="menu__card-button">Cold Dishes</button>
      <button class="menu__card-button">Style Dishes</button>
      <button class="menu__card-button">Hot Dishes</button>
      <button class="menu__card-button">Dumplings</button>
      <button class="menu__card-button">Drinks</button>
    </div>
  </section>
</template>


<script>
  export default {};
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
    border-radius: 2px;
    display: flex;
    align-items: flex-start;
    justify-content: center;

    &-button {
      display:inline-block;
      padding:0.46em 1.6em;
      border:0.1em solid $color-black;
      margin:0 0.2em 0.2em 0;
      border-radius:0.12em;
      box-sizing: border-box;
      text-decoration:none;
      font-family:'Roboto',sans-serif;
      font-weight:300;
      font-size: 2rem;
      color: $color-black;
      text-align:center;

      &:hover {
        color: $color-white;
        background-color: $color-black;
      }
    }
  }
}

</style>