<template>
  <div class="footer">
    <div class="navbar_footer">
      <div class="navbar_footer_logo_container">
        <a href="#">
          <img src="@/assets/images/avada-music-logo.png" alt="" />
        </a>
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

    <div class="copy_nlinks">
      <div class="copyrights">
        <p class="small_text">
        ©Copyright 2012 - 2020 | AVADA THEME BY THEMEFUSION | ALL RIGHTS RESERVED | POWERED BY WORDPRESS  
        </p>
      </div>

      <div class="links">
        <a href="#">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="#">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="#">
          <i class="fab fa-instagram"></i>
        </a>
        <a href="#">
          <i class="fab fa-youtube"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    hamburgerMenuList: Array,
    liActive: Function
  },
};
</script>

<style>
</style>