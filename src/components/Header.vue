<template>
  <header>

    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="menu">
        <nav>
          <ul>
            <li><a href=""></a></li>
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
  background-color: aqua;

  .container{
    width: 70%;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;

    .logo img{
      width: 65px;
    
    }

  }

}

</style>