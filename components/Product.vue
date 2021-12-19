<template>
<b-container class="mt-4" fluid>
    <b-row>
      <b-col v-for="prdt in products" :key="prdt.key" cols="3">
        <b-card
          :title="prdt.name"
          img-src="https://picsum.photos/600/300/?image=25"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem"
          class="mb-2"
        >
          <b-card-text>₹ {{prdt.price}}</b-card-text>

          <b-button href="#" variant="success">Buy</b-button>
        </b-card>
      </b-col>
    </b-row>
    </b-container>
</template>

<script>
export default {
    props: ['products']

}
</script>
