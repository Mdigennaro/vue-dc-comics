<template>

  <main>

    <section class="main-top">
      <div class="container">
        <h2>--> Content goes here &lt;-- </h2>
      </div>
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

main{
  .main-top{
    height: 100px;
    background-color: black;
    display: flex;
    align-content: center;
  
    h2{
      font-size: 20px;
      color: white;
      font-weight: bold;
    }
  }

  .main-bottom{
    height: 120px;
    background-color: #0282f9;
    display: flex;
    align-content: center;

    ul{
      width: 100%;
      list-style:none;
      display: flex;
      align-items: center;
      justify-content: space-around;

      li a{
        display: flex;
        align-items: center;
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