<template>
  <div id="app">
    <Header>
      <!-- navbar -->
      <!-- hamburgher menu -->
    </Header>

    <Main>
      <!-- Sezione Hero
        titolo
        sottotitolo
        bottoni link -->

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
