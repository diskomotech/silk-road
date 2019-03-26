<template>
  <div id="nav" class="nav">
    <router-link to="/" class="nav__logo">Silk Road</router-link>
    <nav>
      <router-link to="/about" class="nav__item">About</router-link>
      <router-link to="/menu" class="nav__item">Menu</router-link>
      <router-link to="/findus" class="nav__item">Find Us</router-link>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 10rem;
  padding: 0 4rem;
  background-color: $color-primary;
  font-size: 2rem;

  &__logo {
    color: $color-white;
  }

  &__item {
    color: $color-secondary;
    padding: 0 2rem;
  }
}
</style>
