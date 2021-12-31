<template>
<div>
  <h1>Choose your products</h1>
  <product :products="products" />
</div>
</template>
<script>
import product from '~/components/Product.vue'
export default {
  name: 'IndexPage',
  components: {
    product
  },
  data () {
    return {
      products: [
      { id: 1, name: 'Apple iphone', price: 100000, category: 'smartPhone', img: '', color: '' },
      { id: 2, name: 'Android TV', price: 25000, category: 'tv', img: '', color: '' },
      { id: 3, name: 'Macbook pro', price: 190000, category: 'laptop', img: '', color: '' },
      { id: 4, name: 'Smart watches', price: 5000, category: 'watches', img: '', color: '' },
      { id: 5, name: 'Shirts', price: 2000, category: 'cloths', img: '', color: '' },
      { id: 6, name: 'shoes', price: 4000, category: 'footware', img: '', color: '' }
      ]
    }
  }
}
</script>
<style>
h1{
  /* background-color: yellow; */
  margin: 1rem 0 0 0;
}
</style>
