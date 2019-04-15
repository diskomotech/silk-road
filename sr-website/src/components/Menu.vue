<template>
  <section class="menu">
    <div class="menu__card">

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
    width: 70vw;
    height: 70vh;
    background-color: $color-white; 
    border-radius: 2px;
  }
}

</style>