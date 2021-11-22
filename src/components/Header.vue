<template>
  <div class="header">
    <div class="navbar">
      <div class="navbar_logo_container">
        <img src="@/assets/images/avada-music-logo.png" alt="" />
      </div>

      <div class="hamburger_menu">
        <div class="hamburger_menu_icon">
          <i class="fas fa-bars"></i>
          <i class="fas fa-times"></i>
        </div>

        <div class="hamburger_menu_expand">
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
          <a href="#">LATEST ALBUM</a>
          <a href="#">LIVE DATES</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
</style>