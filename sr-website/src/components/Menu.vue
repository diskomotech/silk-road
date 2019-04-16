<template>
  <section class="menu">
    <div class="menu__card">
      <button class="menu__card-button">View Menu</button>
    </div>
  </section>
</template>

<script>
  export default {};
</script>

<style lang="scss">
.menu {
  background-image: url("../assets/images/lantern2.jpeg");
  background-size: cover;
  background-position: center center;
  position: relative;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;

  &__card {
    width: 50vw;
    height: 60vh;
    background-color: $color-white; 
    border-radius: 2px;

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
      font-size: 2.4rem;
      color:$color-black;
      text-align:center;

      &:hover {
        color: $color-white;
        background-color: $color-black;
      }
    }
  }
}

</style>