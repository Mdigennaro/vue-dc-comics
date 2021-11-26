<template>
  <header>

    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu">
        <nav>
          <ul>
            <li v-for="(item,index) in links" :key="index">
              <a @click="item.active == !item.active" :class="{active: item.active}" :href="item.url">{{item.text}}</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>

  </header>
</template>

<script>
export default {
  name: "Header",

  data(){
    return {
      links:[
        {
          url: '/',
          text: 'characters',
          active: false
        },
        {
          url: '/',
          text: 'comics',
          active: false
        },
        {
          url: '/',
          text: 'movies',
          active: false
        },
        {
          url: '/',
          text: 'tv',
          active: false
        },
        {
          url: '/',
          text: 'games',
          active: false
        },
        {
          url: '/',
          text: 'collectibles',
          active: false
        },
        {
          url: '/',
          text: 'videos',
          active: false
        },
        {
          url: '/',
          text: 'fans',
          active: false
        },
        {
          url: '/',
          text: 'news',
          active: false
        },
        {
          url: '/',
          text: 'shop',
          active: false
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";

header{

  height: 100px;
  display: flex;
  align-items: center;

  .logo img{
    width: 65px;
  }

  nav ul{
    list-style: none;
    @include allCenter();

    li a{
      margin: 10px;
      text-decoration: none;
      color: rgb(58, 58, 58);
      text-transform: uppercase;
      font-size: 10px;
      font-weight: bold;
      padding-bottom: 37px;
      &:hover, &.active{
        color: $primary-color;
        border-bottom: 4px solid $primary-color;
      }
    }
  }

}

</style>