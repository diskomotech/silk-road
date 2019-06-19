<template>
  <div>
    <div v-for="item in items">
      <span class="menu__dish-name">{{item.name}}</span>
      <br/>
      <span class="menu__dish-desc">{{item.desc}}</span>
      <br/>
      <span class="menu__dish-price">{{item.price}}</span>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          {
            name: 'Mix Shreds Salad',
            veg: true,
            desc: 'Carrot vermicelli & spinach in hot & sour sauce',
            price: 3
          },
          {
            name: 'Xinjiang Spicy Salad',
            veg: true,
            desc: 'Onion, green chilli, tomato & coriander',
            price: 3
          },
          {
            name: 'Cucumber in Sauce',
            veg: true,
            desc: 'Cucumber cubes in special sauce',
            price: 3
          },
          {
            name: 'Shredded Kelp',
            veg: true,
            desc: 'Shredded kelp in hot sauce',
            price: 3
          },
          {
            name: 'Pork with Garlic Sauce',
            veg: false,
            desc: 'Sliced belly pork in hot sauce',
            price: 4
          },
          {
            name: 'Assorted Spiced Beef',
            veg: false,
            desc: 'Sliced spiced beef in a special sauce with chilli oil',
            price: 4
          },
          {
            name: 'Ox Tripe in Chilli Sauce',
            veg: false,
            desc: 'Shredded tripe in a tasty chilli sauce',
            price: 4
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
