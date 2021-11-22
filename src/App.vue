<template>
  <div id="app">
    <Header
    :hamburgerMenuList="hamburgerMenuList">
      <!-- navbar -->
      <!-- hamburgher menu -->

       <!-- Sezione Hero
        titolo
        sottotitolo
        bottoni link -->

    </Header>

    <Main>
     
      <!-- Sezione Brake
        titolo
        sottotitolo -->

      <!-- Sezione Notizie 
        titolo
        sottotitolo
        cards notizie-->

      <!-- Sezione Play Sample 
        testo
        bottone play-->

      <!-- Sezione Live Dates 
        titolo
        sottotitolo
        ul delle date
        li accordion-->
    </Main>

    <Footer>
      <!-- navbar footer -->
      <!-- copyright e social link -->
    </Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data(){
    return{
      hamburgerMenuList: [
        "Home",
        "Meet The Band",
        "Live Dates",
        "Latest News",
        "Albums",
        "Fans"
      ]
    }
  }
};
</script>

<style lang="scss">
@import "styles/header";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
