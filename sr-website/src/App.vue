<template>
  <div id="app">
    <NavBar/>
    <router-view/>
    <Intro/>
    <About/>
    <Menu/>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Intro from "@/components/Intro.vue";
import About from "@/components/About.vue";
import Menu from "@/components/Menu.vue";

export default {
  components: {
    NavBar,
    Intro,
    About,
    Menu
  }
};
</script>
