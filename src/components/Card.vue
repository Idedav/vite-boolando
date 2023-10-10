<script>
export default {
    name:'Card'
}
</script>


<template>

    <div class="product">
        <div class="img-product">
          <img src="/public/1.webp" alt="" class="imgdefault">
          <img src="/public/1b.webp" alt="" class="imghover">
          <span class="heart">&hearts;</span>
          <div class="target">
            <span class="discount">-50%</span>
            <span class="sustain">Sostenibilità</span>
          </div>
        </div>
        <div class="description">
          <span>Levi's</span>
          <h3><strong>RELAXED FIT TEE UNISEX</strong></h3>
        </div>
        <div class="price">
          <span class="discounted">14,99 &euro;</span>
          <span class="original">29,99 &euro;</span>
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