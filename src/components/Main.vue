<template>

  <main>

    <section class="main-top">
      <div class="container">
        <h2>--> Content goes here &lt;-- </h2>
      </div>
    </section>

    <section class="main-center">

      <div class="container-dc">
        <div class="container">
          <h3>Current series</h3>
            <div class="box-fumetti">
              <Fumetto v-for="(fumetto, index) in listaFumetti" :key="index"
              :imgFumetto="fumetto.thumb" 
              :nomeFumetto="fumetto.series" 
              />
            </div>
            <div class="btn">Load more</div>
        </div>
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
import Fumetto from './Fumetti.vue';

export default {
  name:"Main",

  components:{
    Fumetto,
  },

  data(){
    return{
      listaFumetti:[
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg? itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";
@import "../assets/style/utilities.scss";

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
      display: flex;
      flex-direction: column;

      .container{
        flex-direction: column;

        h3{
          align-self: flex-start;
          color: white;
          font-weight: bold;
          text-transform: uppercase;
          background-color: $primary-color;
          padding: 10px;
          margin-top: -20px;
          font-size: 20px;
          margin-bottom: 30px;
        }

        .box-fumetti{
          @include allCenter();
          justify-content: space-between;
          flex-wrap: wrap;
          
        }

        .btn{
          color: white;
          font-weight: bold;
          text-transform: uppercase;
          background-color: $primary-color;
          padding: 10px 40px;
          font-size: 14px;
          cursor: pointer;
        }

      }

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