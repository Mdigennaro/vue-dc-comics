<template>
  <header>

    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu">
        <nav>
          <ul>
            <li><a href="#">characters</a></li>
            <li><a href="#">comics</a></li>
            <li><a href="#">movies</a></li>
            <li><a href="#">tv</a></li>
            <li><a href="#">games</a></li>
            <li><a href="#">collectibles</a></li>
            <li><a href="#">videos</a></li>
            <li><a href="#">fans</a></li>
            <li><a href="#">news</a></li>
            <li><a href="#">shop</a></li>
          </ul>
        </nav>
      </div>
    </div>

  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style lang="scss">

header{

  height: 100px;
  display: flex;
  align-items: center;

  .logo img{
    width: 65px;
  }

  nav ul{
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;

    li a{
      margin: 10px;
      text-decoration: none;
      color: rgb(58, 58, 58);
      text-transform: uppercase;
      font-size: 10px;
      font-weight: bold;
      padding-bottom: 37px;
      &:hover, &.active{
        color: #0282f9;
        border-bottom: 4px solid #0282f9;
      }
    }
  }

  

}

</style>