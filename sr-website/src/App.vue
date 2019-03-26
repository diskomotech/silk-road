<template>
  <div id="app">
    <NavBar/>
    <router-view/>
    <Intro/>
    <About/>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Intro from "@/components/Intro.vue";
import About from "@/components/About.vue";

export default {
  components: {
    NavBar,
    Intro,
    About
  }
};
</script>
