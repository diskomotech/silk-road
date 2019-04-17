<template>
  <div>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        cold: [
          {
            name: 'Mix Shreds Salad',
            veg: true,
            desc: 'Carrot vermicelli & spinach in a hot & sour sauce',
            price: 3
          },
          {
            name: 'Xinjiang Spicy Salad',
            veg: true,
            desc: 'Onion, green chilli, tomato & coriander',
            price: 3
          },
        ],
        style: [
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
        ],
        hot: [
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
        ],
        dumplings: [
          {
            name: 'Lamb & Onion Filling',
            veg: false,
            desc: '',
            price: 3
          },
          {
            name: 'Beef & Onion Filling',
            veg: false,
            desc: '',
            price: 3
          },
        ],
        drinks: [
          {
            name: 'Coke',
            veg: false,
            desc: '',
            price: 1
          },
          {
            name: 'Diet Coke',
            veg: false,
            desc: '',
            price: 1
          },
        ]
      }
    }
  }
</script>

<style lang="scss">

</style>