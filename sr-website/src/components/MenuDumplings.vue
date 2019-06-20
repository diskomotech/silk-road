<template>
  <div>
    <div v-for="item in items">
      <span class="menu__dish-content menu__dish-name">{{item.name}}</span>
      <br/>
      <span class="menu__dish-content menu__dish-price">£{{item.price}}</span>
      <hr>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          {
            name: 'Lamb & Onion Filling',
            veg: false,
            price: 3
          },
          {
            name: 'Beef & Onion Filling',
            veg: false,
            price: 3
          },
          {
            name: 'Pork & Celery Filling',
            veg: false,
            price: 3
          },
          {
            name: 'Egg, Leek & Shrimp Filling',
            veg: false,
            price: 3.50
          },
          {
            name: 'Fried Dumpling',
            veg: false,
            price: 3.50
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
