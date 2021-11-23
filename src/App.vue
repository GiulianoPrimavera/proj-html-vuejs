<template>
  <div id="app">
    <Header
    :hamburgerMenuList="hamburgerMenuList"
    >
    </Header>

    <Main
    :liveDatesEvents="liveDatesEvents"
    >
     
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
      ],
      liveDatesEvents: [
        {
          date: "17/08/2020",
          position: "GEM FESTIVAL 2020 ANAKALIA, GEORGIA"
        },
        {
          date: "24/09/2020",
          position: "groovefest dominical republic"
        },
        {
          date: "31/10/2020",
          position: "oasis festival 2020 Marrakech, Morocco"
        },
        {
          date: "07/11/2020",
          position: "moga festival - Essaouria, Morocco"
        },
        {
          date: "10/12/2020",
          position: "Envision Festival -Uvita, Costa Rica"
        }
      ]
    }
  }
};
</script>

<style lang="scss">
@import "styles/app";
@import "styles/header";
@import "styles/main";
</style>
