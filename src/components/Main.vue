<template>

  <main>

    <section class="main-top">
      <div class="container">
        <h2>--> Content goes here &lt;-- </h2>
      </div>
    </section>

    <section class="main-center">

      <div class="container-dc"></div>

    </section>

    <section class="main-bottom">
      <div class="container">
        <ul>
          <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt="">Digital comics</a></li>
          <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt="">dc merchandise</a></li>
          <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt="">subscription</a></li>
          <li><a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt="">comic shop locator</a></li>
          <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="">dc power visa</a></li>
        </ul>
      </div>
    </section>

  </main>
  
</template>

<script>
export default {
  name:"Main"
}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";

main{
  .main-top{
    height: 100px;
    background-color: black;
    @include allCenter();
  
    h2{
      font-size: 20px;
      color: white;
      font-weight: bold;
      cursor:pointer;
    }
  }

  .main-center{
    width: 100%;
    height: 900px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    position: relative;

    .container-dc{
      position: absolute;
      bottom: 0px;
      width: 100%;
      height: 62%;
      background-color: #1c1c1c;
    }

  }

  .main-bottom{
    height: 120px;
    background-color: $primary-color;
    @include allCenter();

    ul{
      width: 100%;
      list-style:none;
      @include allCenter();
      justify-content: space-around;

      li a{
        @include allCenter();
        text-decoration: none;
        color: white;
        text-transform: uppercase;
        font-size: 13px;

        img{
          width: 35px;
          margin: 10px;
        }
      }
    }
  }
}

</style>