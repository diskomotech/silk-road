<template>
  <div>
    <div v-for="item in items">
      <span class="menu__dish-content menu__dish-name">{{item.name}}</span>
      <br/>
      <span class="menu__dish-content menu__dish-desc" v-if="(item.desc)">{{item.desc}}</span>
      <br v-if="(item.desc)"/>
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
            name: 'Cabbage in Vinegar Sauce',
            veg: true,
            desc: '',
            price: 5
          },
          {
            name: 'Hot & Sour Shredded Potato',
            veg: true,
            desc: '',
            price: 5
          },
          {
            name: 'Extra Hot Chinese Leaves',
            veg: true,
            desc: 'Stir fried cabbage slices in a extra hot sauce',
            price: 5
          },
          {
            name: 'Home Style Aubergine',
            veg: true,
            desc: 'Stir fried aubergines with tomato & green chilli',
            price: 5.50
          },
          {
            name: 'Garlic Pak-Choi',
            veg: true,
            desc: 'Stir-fried pak-choi in garlic sauce',
            price: 5.50
          },
          {
            name: 'Home Style Cabbage',
            veg: true,
            desc: 'Stir-fried cabbage and dried chilli',
            price: 5.50
          },
          {
            name: 'Stir Fried Spinach',
            veg: true,
            desc: '',
            price: 7
          },
          {
            name: 'Pork with Black Fungus',
            veg: false,
            desc: 'Pork slices, black fungus & cabbage',
            price: 7
          },
          {
            name: 'Yu-Shiang Shredded Pork',
            veg: false,
            desc: 'Shredded pork, carrot, black fungus & red chilli giving a fish-like sour & sweet taste',
            price: 7
          },
          {
            name: 'Chicken with Green Chilli',
            veg: false,
            desc: 'Chicken cubes with green chilli & red chilli',
            price: 7
          },
          {
            name: 'Beef with Pistachio',
            veg: false,
            desc: '',
            price: 7
          },
          {
            name: 'Pepper with Shredded Tripe',
            veg: false,
            desc: '',
            price: 7
          },
          {
            name: 'Double Cooked Pork Slices',
            veg: false,
            desc: 'A traditional si-chuon dish with pork belly',
            price: 7
          },
          {
            name: 'Lamb Slices with Spring Onion',
            veg: false,
            desc: '',
            price: 8
          },
          {
            name: 'Stir Fried Chicken Gizzards',
            veg: false,
            desc: 'Chicken gizzards & onion fried with cumin & chilli powder',
            price: 8
          },
          {
            name: 'Xingjiang Style Noodle in Soup',
            veg: false,
            desc: 'A bowl of sour soup with hand-pulled noodles, lamb & tomato',
            price: 4.50
          },
          {
            name: 'Boiled Rice',
            veg: true,
            desc: '',
            price: 1.80
          },
          {
            name: 'Belt Noodle',
            veg: true,
            desc: '',
            price: 2
          },
          {
            name: 'Hand-Pulled Noodle',
            veg: true,
            desc: '',
            price: 2
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
