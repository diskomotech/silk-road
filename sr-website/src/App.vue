<template>
  <div id="app">
    <NavBar/>
    <router-view/>
    <Intro/>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Intro from "@/components/Intro.vue";

export default {
  components: {
    NavBar,
    Intro
  }
};
</script>
