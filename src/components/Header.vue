<script>
export default {
    name:'Header'
}
</script>


<template>
  <header>
    <div class="container">

      <nav>
        <ul>
          <li><a href="#">Donna</a></li>
          <li><a href="#">Uomo</a></li>
          <li><a href="#">Bambini</a></li>
        </ul>
      </nav>

      <div class="logo">
        <img src="/public/boolean-logo.png" alt="">
      </div>

      <div class="icons">
        <a href="#"><i class="fa-regular fa-user"></i></a>
        <a href="#"><i class="fa-regular fa-heart"></i></a>
        <a href="#"><i class="fa-solid fa-bag-shopping"></i></a>
      </div>

    </div>
  </header>
</template>


<style lang="scss" scoped>
@use '../scss/partials/variabeles.scss' as *;

header {
  background-color: $back-ground-header;
  height: 100px;
  .container {
    display: flex;
    justify-content: space-between;
    nav {
      line-height: 100px;
      ul {
        list-style: none;
        li {
          display: inline-block;
          a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
            margin-right: 15px;
          }
        }
      }
    }
    .logo{
      width: 200px;
      display: flex;
      justify-content: center;
      align-items: center;
      img{
        width: 100%;
      }
    }
    .icons{
      line-height: 100px;
      a{
        color: white;
        font-size: 1.2rem;
        margin-left: 15px;
      }
    }

  }
}


</style>