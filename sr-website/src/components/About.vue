<template>
  <section class="about">
    <div class="empty"></div>

    <div class="about__content">
      <h3>About Us</h3>
      <p
        class="about__text"
      >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Turpis egestas pretium aenean pharetra magna ac placerat. Lectus proin nibh nisl condimentum. Eu mi bibendum neque egestas congue quisque egestas diam in. Erat imperdiet sed euismod nisi porta lorem mollis aliquam ut. Malesuada proin libero nunc consequat interdum varius sit amet. Arcu non sodales neque sodales ut etiam sit amet. Eget mi proin sed libero. Eget mi proin sed libero enim sed. Posuere morbi leo urna molestie at elementum eu. Aliquet porttitor lacus luctus accumsan tortor posuere ac. Nunc lobortis mattis aliquam faucibus purus in massa tempor nec. Faucibus turpis in eu mi bibendum neque egestas congue quisque. Consequat semper viverra nam libero justo. Commodo sed egestas egestas fringilla. Rutrum quisque non tellus orci ac.</p>
      <p>Id volutpat lacus laoreet non curabitur gravida. Suspendisse sed nisi lacus sed viverra tellus. Venenatis cras sed felis eget velit aliquet sagittis id. Senectus et netus et malesuada fames ac. Neque viverra justo nec ultrices. Interdum velit laoreet id donec ultrices. Commodo quis imperdiet massa tincidunt nunc pulvinar. Enim ut sem viverra aliquet eget sit amet tellus. Egestas integer eget aliquet nibh praesent tristique magna. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus mauris. Ac turpis egestas sed tempus urna et pharetra pharetra massa. Semper feugiat nibh sed pulvinar. Libero justo laoreet sit amet cursus sit amet dictum sit. Eget est lorem ipsum dolor sit.</p>
    </div>

    <div class="empty"></div>

    <div>
      <img
        src="../assets/images/image.jpg"
        alt="Waitress carrying plate of delicious food"
        class="about__img"
      >
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
.about {
  height: 100vh;
  display: grid;
  grid-template-columns: 8rem 1fr 8rem 1fr;
  align-items: center;
  background-color: $color-white;

  &__content {
    color: $color-black;
    font-size: 1.5rem;
  }

  &__img {
    width: 47rem;
  }
}
</style>
