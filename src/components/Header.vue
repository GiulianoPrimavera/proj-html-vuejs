<template>
  <div class="header">
    <div class="navbar">
      <div class="navbar_logo_container">
        <a href="#">
          <img src="@/assets/images/avada-music-logo.png" alt="" />
        </a>
      </div>

      <div class="hamburger_menu">
        <div class="hamburger_menu_icon" @click="hamburgerMenu">
          <i class="fas fa-bars icon_active"></i>
        </div>

        <div class="hamburger_menu_collapse" @click="hamburgerMenu">
          <div class="navbar_logo_container">
            <a href="#">
              <img src="@/assets/images/avada-music-logo.png" alt="" />
            </a>
          </div>

          <div class="hamburger_menu_icon">
            <i class="fas fa-times"></i>
          </div>

          <ul>
            <li
              v-for="(item, i) in hamburgerMenuList"
              :key="i"
              :class="item.state ? 'item_state_active' : ''"
              @click="liActive(i), $emit('itemIndex', i)"
            >
              <a href="#">{{ item.title }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>

    <div class="hero">
      <div class="hero_text">
        <h1>Untold Stories</h1>

        <p class="big_text">
          <em>There is an untold story behind every favorite song.</em>
        </p>

        <div class="hero_buttons">
          <a href="#" id="latest_album" class="hero_focus" @click="buttonFocus"
            ><strong>LATEST ALBUM</strong></a
          >
          <a href="#" id="live_dates" @click="buttonFocus"
            ><strong>LIVE DATES</strong></a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    hamburgerMenuList: Array,
    liActive: Function
  },
  methods: {
    hamburgerMenu() {
      //quando viene premuta l'icona viene visualizzata l'altra icona e viene visualizzato l'hamburger menu espanso
      const hamMenuBars = document.querySelector(".fa-bars");
      const hamMenuTimes = document.querySelector(".fa-times");
      const hamMenuExpand = document.querySelector(".hamburger_menu_collapse");
      hamMenuBars.classList.toggle("icon_active");
      hamMenuTimes.classList.toggle("icon_active");
      hamMenuExpand.classList.toggle("hamburger_menu_expand");
    },
    buttonFocus() {
      const latestAlbum = document.getElementById("latest_album");
      const liveDates = document.getElementById("live_dates");
      latestAlbum.classList.toggle("hero_focus");
      liveDates.classList.toggle("hero_focus");
    },
  }
};
</script>

<style>
</style>