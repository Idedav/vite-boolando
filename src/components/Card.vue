<script>
export default {
    name:'Card',
    props:{
      productObj: Object
    }
}
</script>


<template>

    <div class="product">
        <div class="img-product">
          <img :src="`/public/${productObj.primaryImage}`" alt="" class="imgdefault">
          <img :src="`/public/${productObj.secondaryImage}`" alt="" class="imghover">
          <span class="heart">&hearts;</span>
          <div class="target">
            <span v-if="productObj.discount != null"
            class="discount">{{ productObj.discount }}</span>
            <span v-if="productObj.sostenibilita === true"
            class="sustain">Sostenibilità</span>
          </div>
        </div>
        <div class="description">
          <span>{{ productObj.marca }}</span>
          <h3><strong>{{ productObj.modello }}</strong></h3>
        </div>
        <div class="price">
          <span class="discounted">{{ productObj.lastPrice }} &euro;</span>
          <span v-if="productObj.fullPrice != null"
          class="original">{{ productObj.fullPrice }} &euro;</span>
        </div>
    </div>

</template>


<style lang="scss" scoped>
@use '../scss/partials/variabeles.scss' as *;
.product {
      margin-bottom: 40px;
      .img-product {
        width: 350px;
        position: relative;
      img {
        width: 100%;
      }
      .heart {
        font-size: 30px;
        position: absolute;
        top: 10px;
        right: 0px;
        padding: 10px;
        background-color: white;
        &:hover{
          color: red;
          cursor: pointer;
        }
      }
      .target {
        position: absolute;
        bottom: 30px;
        left: 0px;
        .discount {
          padding: 5px 10px;
          background-color: $discount-color;
          color: white;
        }
        .sustain{
          padding: 5px 10px;
          background-color: $flag-color;
          color: white;
        }
      }
    }
    .imghover {
      display: none;
    }
  
    .price {
      font-weight: bold;
      .discounted { 
      color: red;
      }
      .original {
      text-decoration: line-through;
      }
    }
    &:hover .imghover{
      display: inline-block;
      cursor: pointer;
    }
    &:hover .imgdefault{
      display: none;
    }
  }

</style>