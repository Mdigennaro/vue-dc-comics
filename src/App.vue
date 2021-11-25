<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }

}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
@import "./assets/style/utilities.scss";
@import "./assets/style/vars.scss";
@import "./assets/style/mixins.scss";

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app{
  width: 100%;
  height: 100vh;
  min-width: 1180px;
  font-family: 'Lato', sans-serif;

}

</style>
