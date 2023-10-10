<script>
export default {
    name:'Main'
}
</script>


<template>
  <main>
    <div class="container">

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

      <div class="product">
        <div class="img-product">
          <img src="/public/2.webp" alt="" class="imgdefault">
          <img src="/public/2b.webp" alt="" class="imghover">
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

      <div class="product">
        <div class="img-product">
          <img src="/public/3.webp" alt="" class="imgdefault">
          <img src="/public/3b.webp" alt="" class="imghover">
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

      <div class="product">
        <div class="img-product">
          <img src="/public/4.webp" alt="" class="imgdefault">
          <img src="/public/4b.webp" alt="" class="imghover">
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

      <div class="product">
        <div class="img-product">
          <img src="/public/5.webp" alt="" class="imgdefault">
          <img src="/public/5b.webp" alt="" class="imghover">
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

      <div class="product">
        <div class="img-product">
          <img src="/public/6.webp" alt="" class="imgdefault">
          <img src="/public/6b.webp" alt="" class="imghover">
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
  }
}

</style>