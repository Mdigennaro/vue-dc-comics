<template>

  <footer>

    <section class="footer-top">
      <div class="container clearfix">

        <div class="ft-left">
          
          <nav>
            <ul>
              <li><h4>dc comics</h4></li>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>

            <ul>
              <li><h4>shop</h4></li>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>

            <ul>
              <li><h4>dc</h4></li>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>

            <ul>
              <li><h4>sites</h4></li>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </nav>

        </div>

        <div class="ft-right">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>

      </div>
    </section>

    <section class="footer-bottom">
      <div class="container">

      <div class="btn">sign-up now!</div>

      <div class="social">
        <h4>Follow us</h4>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
      </div>

      </div>
    </section>

  </footer>

</template>

<script>
export default {

  name: "Footer"

}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";

footer{
  height: calc(100% - 320px);

  .footer-top{
    width: 100%;
    height: calc(100% - 90px);
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    @include allCenter();
    overflow: hidden;

    .ft-left{
      float: left;
      width: 50%;
      height: 100%;
      overflow: hidden;
      
      nav{
        max-height: 300px;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;

        ul{
          list-style: none;

          h4{
            color: white;
            text-transform: uppercase;
            margin: 7px 0;
            font-weight: bold;
            font-size: 15px;
          }

          li a{
            color:rgb(104, 104, 104);
            text-decoration: none;
            font-size: 10px;
          }
            
        }
      }
    }

    .ft-right{
      float: left;
      width: 50%;

      img{
        width: 100%;
      }
    }

  }

  .footer-bottom{
    width: 100%;
    height: 90px;
    background-color: #303030;
    @include allCenter();

    .btn{
      color: white;
      font-size: 13px;
      font-weight: bold;
      text-transform: uppercase;
      border: 2px solid $primary-color;
      padding: 10px;
      cursor: pointer;
    }

    .social{
      @include allCenter();

      h4{
        color: $primary-color;
        text-transform: uppercase;
        margin: 10px;
      }

      img{
        margin: 5px;
        cursor: pointer;
      }
    }
  }
}


</style>