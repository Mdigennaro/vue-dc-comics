<template>

<div class="fumetto-singolo">
  <div class="fumetto-cover">
    <img :src="imgFumetto" alt="">
  </div>
  
  <h4>{{nomeFumetto}}</h4>
</div>
  
</template>

<script>
export default {
  nome: "Fumetti",
  props:{
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
  flex-basis: calc(100% / 6 - 10px);
  height: 225px;
  padding: 10px;

  .fumetto-cover{
    overflow: hidden;
    margin-bottom: 15px;
    height: 150px;
    
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