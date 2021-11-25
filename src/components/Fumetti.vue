<template>

<div class="fumetto-singolo">
  <div class="fumetto-cover">
    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
  </div>
  
  <h4>Action Comics</h4>
</div>
  
</template>

<script>
export default {
  nome: "Fumetti",
  promps:{
    imgFumetto: String,
    nomeFumetto: String

  }
}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";
@import "../assets/style/utilities.scss";

.fumetto-singolo{
  flex-basis: calc(100% / 6);
  height: 225px;
  padding: 10px;

  .fumetto-cover{
    height: 150px;
    overflow: hidden;
    margin-bottom: 15px;
    
    img{
      width: 100%;
    }
  }

  h4{
    color: white;
    font-size: 11px;
    font-weight: lighter;
    text-transform: uppercase;
  }

}

</style>