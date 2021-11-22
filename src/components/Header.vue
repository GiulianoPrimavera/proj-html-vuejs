<template>
  <div class="header">
    <div class="navbar">
      <div class="navbar_logo_container">
        <img src="@/assets/images/avada-music-logo.png" alt="" />
      </div>

      <div class="hamburger_menu">
        <div class="hamburger_menu_icon" @click="hamburgerMenu">
          <i class="fas fa-bars icon_active"></i>
          <i class="fas fa-times"></i>
        </div>

        <div class="hamburger_menu_collapse">
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Meet The Band</a></li>
            <li><a href="#">Live Dates</a></li>
            <li><a href="#">Latest News</a></li>
            <li><a href="#">Albums</a></li>
            <li><a href="#">Fans</a></li>
          </ul>
        </div>
      </div>
    </div>

    <div class="hero">
      <div class="hero_text">
        <h1>Untold Stories</h1>

        <p><em>There is an untold story behind every favorite song.</em></p>

        <div class="hero_buttons">
          <a href="#" id="latest_album" class="hero_focus"  @click="buttonFocus">LATEST ALBUM</a>
          <a href="#" id="live_dates"  @click="buttonFocus">LIVE DATES</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
      hamburgerMenu(){
          //quando viene premuta l'icona viene visualizzata l'altra icona e viene visualizzato l'hamburger menu espanso
          const hamMenuBars = document.querySelector(".fa-bars");
          const hamMenuTimes = document.querySelector(".fa-times");
          const hamMenuExpand = document.querySelector(".hamburger_menu_collapse")
          hamMenuBars.classList.toggle("icon_active");
          hamMenuTimes.classList.toggle("icon_active");
          hamMenuExpand.classList.toggle("hamburger_menu_expand");

          const navBar = document.querySelector(".navbar")
          navBar.classList.toggle("navbar_bg_red")
      },
      buttonFocus(){
          const latestAlbum = document.getElementById("latest_album")
          const liveDates = document.getElementById("live_dates")
          latestAlbum.classList.toggle("hero_focus")
          liveDates.classList.toggle("hero_focus")
      }
  }
};
</script>

<style>
</style>