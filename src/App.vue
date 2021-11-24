<template>
  <div id="app">
    <Header />
    <Main />
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main
  }

}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
@import "./assets/style/utilities.scss";

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app{
  width: 100%;
  min-width: 1180px;
  font-family: 'Lato', sans-serif;

}

</style>
