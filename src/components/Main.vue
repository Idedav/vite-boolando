<script>
import Card from './Card.vue';
export default {
    name:'Main',
    components:{
      Card
    }
}
</script>


<template>
  <main>
    <div class="container">
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
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