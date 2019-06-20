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
            name: 'Xinjiang Lamb Shish',
            veg: false,
            desc: 'Fresh lamb pieces & fat roasted over charcoal, seasoned with salt, cumin & chilli powder. Served on steel skewer',
            price: 1
          },
          {
            name: 'Ox Tripe Shish',
            veg: false,
            desc: 'Tripe slices roasted over charcoal, seasoned with salt, cumin & chilli powder. Served on steel skewer',
            price: 1
          },
          {
            name: 'Kidney Shish',
            veg: false,
            desc: 'Lamb kidney roasted over charcoal, seasoned with soft, cumin & chili powder, served on steel skewer',
            price: 1.50
          },
          {
            name: 'Fish Shish',
            veg: false,
            desc: 'Boneless red snapper roasted over charcoal, seasoned with salt, cumin & chilli powder, served on steel skewer',
            price: 2.50
          },
          {
            name: 'Big Plate Chicken',
            veg: false,
            desc: 'Most popular xinjiang dish in china, contain chicken with bone, potato green chilli & dried chili, including a protein of belt noodle',
            price: 15
          },
          {
            name: 'Middle Plate Chicken',
            veg: false,
            desc: 'Smaller version of big plate chicken',
            price: 9
          },
          {
            name: 'Special Big Plate Chicken',
            veg: false,
            desc: 'Another version of big plate chicken,contains chicken with bone, dried chilli & green chilli',
            price: 28
          },
          {
            name: 'Big Plate Tripe',
            veg: false,
            desc: 'Tripe slices with onion & green chili in a special seasoning',
            price: 12
          },
          {
            name: 'Boiled Lamb',
            veg: false,
            desc: 'Boiled lamb with bone covered with a salty onion sauce, use of hands are recommended',
            price: 12
          },
          {
            name: 'T.E.P. Noodle',
            veg: true,
            desc: 'Tomato, egg & pepper covered on hand-pulled noodle',
            price: 6
          },
          {
            name: 'Mixed Vegetable with Noodle',
            veg: true,
            desc: 'Onions, Chinese leaves, celery, tomato & pepper covered on hand-pulled noodle',
            price: 6
          },
          {
            name: 'Special Cooked Lamb with Noodle',
            veg: false,
            desc: 'A stir fried lamb dish with a similar flavor of lamb shish seasoned with salt, cumin & chili powder covered on hand-pulled noodle',
            price: 6.50
          },
          {
            name: 'Cabbage & Lamb with Noodle',
            veg: false,
            desc: 'Cabbage slices & lamb covered on hand pulled noodle',
            price: 6.50
          },
          {
            name: 'Luxury Noodle',
            veg: false,
            desc: 'Special cooked lamb with noodle & a fried egg on both sides',
            price: 7
          },
          {
            name: 'Xinjiang Style Fried Noodle',
            veg: false,
            desc: 'Stir fried hand-pulled noodle with lamb, celery, onions tomato & chilli',
            price: 6.50
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
