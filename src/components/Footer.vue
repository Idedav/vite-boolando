<script>
export default {
    name:'Footer'
}
</script>


<template>
  <footer>
    <div class="container">

      <div class="reference">
        <h3>Boolando s.r.l.</h3>
        <div class="links">
          <a href="#">Informazioni legali</a>
          <a href="#">Informativa sulla privacy</a>
          <a href="#">Diritto di recesso</a>
        </div>
      </div>

      <div class="socials">
        <h4>Trovaci anche su</h4>
          <div class="icon">
            <a href="#"><i class="fa-brands fa-square-twitter"></i></a>
            <a href="#"><i class="fa-brands fa-square-facebook"></i></a>
            <a href="#"><i class="fa-brands fa-square-instagram"></i></a>
            <a href="#"><i class="fa-brands fa-square-pinterest"></i></a>
            <a href="#"><i class="fa-brands fa-square-youtube"></i></a>
          </div>
      </div>

    </div>
  </footer>
</template>


<style lang="scss" scoped>
@use '../scss/partials/variabeles.scss' as *;

footer{
  background-color: $back-ground-footer;
  height: 200px;
  color: white;
  .container {
    display: flex;
    justify-content: space-between;
    .reference{
      height: 200px;
      display: flex;
      flex-direction: column;
      justify-content: center;

      h3 {
        font-size: 1.5rem;
        margin-bottom: 10px;
      }
      .links a{
        color: white;
        text-decoration: none;
        font-size: 1.2rem;
      }
    }
    .socials{
      height: 200px;
      display: flex;
      flex-direction: column;
      justify-content: center;

      h4{
        font-size: 1.5rem;
        margin-bottom: 10px;
      }

      a{
        color: white;
        font-size: 2rem;
        margin-right: 15px;
      }
    }
  }
}

</style>