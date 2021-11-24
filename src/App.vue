<template>
  <div id="app">
    <Header
      :hamburgerMenuList="hamburgerMenuList"
      :liActive="liActive"
      @itemIndex="index"
    ></Header>

    <Main :liveDatesEvents="liveDatesEvents"></Main>

    <Footer 
    :hamburgerMenuList="hamburgerMenuList" 
    :liActive="liActive"
    @itemIndex="index"
    ></Footer>
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
  data() {
    return {
      hamburgerMenuList: [
        {
          title: "Home",
          state: true,
        },
        {
          title: "Meet The Band",
          state: false,
        },
        {
          title: "Live Dates",
          state: false,
        },
        {
          title: "Latest News",
          state: false,
        },
        {
          title: "Albums",
          state: false,
        },
        {
          title: "Fans",
          state: false,
        },
      ],
      liveDatesEvents: [
        {
          date: "17/08/2020",
          position: "GEM FESTIVAL 2020 ANAKALIA, GEORGIA",
          itemClickato: false,
        },
        {
          date: "24/09/2020",
          position: "groovefest dominical republic",
          itemClickato: false,
        },
        {
          date: "31/10/2020",
          position: "oasis festival 2020 Marrakech, Morocco",
          itemClickato: false,
        },
        {
          date: "07/11/2020",
          position: "moga festival - Essaouria, Morocco",
          itemClickato: false,
        },
        {
          date: "10/12/2020",
          position: "Envision Festival -Uvita, Costa Rica",
          itemClickato: false,
        },
      ],
    };
  },
  methods: {
    liActive(index) {
      //questo ciclo mette lo state a false per ogni elemento della lista che è a true
      for (let i = 0; i < this.hamburgerMenuList.length; i++) {
        if (this.hamburgerMenuList[i].state === true) {
          this.hamburgerMenuList[i].state = false;
        }
      }
      //qui metto lo stato a true dell'elemento cliccato
      this.hamburgerMenuList[index].state = true;
    },
  }
};
</script>

<style lang="scss">
@import "styles/app";
@import "styles/header";
@import "styles/main";
@import "styles/footer";
</style>
