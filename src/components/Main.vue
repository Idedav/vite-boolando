<script>
import products from '../data/products'
import Card from './Card.vue';
export default {
    name:'Main',
    components:{
      Card
    },
    data(){
      return{
        products
      }
    }
}
</script>


<template>
  <main>
    <div class="container">
      <Card v-for="product in products" :key="product.id" :productObj="product"/>
    </div>
  </main>
</template>


<style lang="scss" scoped>
@use '../scss/partials/variabeles.scss' as *;
main{
  padding-top: 100px;
  .container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    margin: 50px auto;
  }
}

</style>