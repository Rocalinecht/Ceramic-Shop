<template>
  <div class="home">
    <div class="box">
      <h1>Ceramic Shop</h1>
      <h2>Make with hands and Love</h2>
</div>


    <Cart/>
</div>

  
</template>

<script>
// @ is an alias to /src
import Cart from '@/components/Cart.vue'

export default {
  name: 'Home',
  components: {
    Cart
  }
}
</script>
<style scoped>
.box{
  background-image: url('~@/assets/img/background.jpg');
  background-attachment:fixed;
  background-size: cover;
  height: 550px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

h1{
  color: white;
  font-size: 3em;
}
h2{
  font-style: italic;
  color: white;
}
</style>