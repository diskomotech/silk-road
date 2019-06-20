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
            name: 'Coke',
            price: 1
          },
          {
            name: 'Diet Coke',
            price: 1
          },
          {
            name: 'Tango',
            price: 1
          },
          {
            name: 'Chinese Jasmine Tea',
            price: 1.50
          },
          {
            name: 'Aloe Water Juice',
            price: 2.50
          },
          {
            name: 'Tsintao Beer',
            price: 2.50
          },
          {
            name: 'House Red Wine',
            price: 12
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
