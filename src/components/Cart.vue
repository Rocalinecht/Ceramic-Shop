<template>
  <div>
    <h2>Products </h2>
    <div class="container">
      <div class="card--group">
        <div v-for="product in products" :key="product.id">
          <b-card
            :title="product.name"
            :img-alt="product.name"
            :img-src="require(`@/assets/img/ceramic${product.id}.jpg`)"
            img-top
            tag="article"
            style="max-width: 20rem;"
            class="mb-2"
          >
          <b-card-text>
            {{product.price}} €
          </b-card-text>
          <b-button href="#" variant="primary">Add to Shopping Cart</b-button>
  </b-card>
</div>
  </div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'Cart',
  props: {
    msg: String
  },
   data(){
    return{
      tickets:{
        products:null,
        total:0,
      },
      counter:0,
      products: [
        {
          id:1,
          img:'@/assets/img/ceramic1.jpg',
          name:'Vase N°201',
          price: 45,
          cart:false,
          quantity:1
        },
         {
          id:2,
          img:'@/assets/img/ceramic2.jpg',
          name:'Vase N°202',
          price: 40,
          cart:false,
          quantity:1
        },
         {
          id:3,
          img:'@/assets/img/ceramic3.jpg',
          name:'Mug N°401',
          price: 25,
          cart:false,
          quantity:1
        },
         {
          id:4,
          img:'@/assets/img/ceramic4.jpg',
          name:'Vase N°203',
          price: 50,
          cart:false,
          quantity:1
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card--group{
  display: flex;
  border:2px solid lightblue;
  justify-content: space-around;
  margin-top: 50px;
  
}
</style>
