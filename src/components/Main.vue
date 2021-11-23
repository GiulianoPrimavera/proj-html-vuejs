<template>
  <div class="main">
    <div class="brake">
      <!-- sezione di testo (si ripete 3 volte nel codice) -->
      <div class="main_text_section">
        <!-- linea rossa -->
        <div class="brake_red_line"></div>

        <h2>Music Is Life</h2>
        <p class="small_text">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos
          ea at explicabo adipisci doloremque quae non quam ab, vitae nisi
          porro, nihil quisquam id vel provident suscipit architecto dolores
          perspiciatis!
        </p>
      </div>
    </div>

    <div class="news">
      <!-- sezione titolo delle news -->
      <div class="main_text_section">
        <h2>Latest Band News</h2>
        <p class="small_text">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos
          ea at explicabo adipisci doloremque quae non quam ab, vitae nisi
          porro, nihil quisquam id vel provident suscipit architecto dolores
          perspiciatis!
        </p>
      </div>

      <!-- contenitore delle news -->
      <div class="news_container">
        <div class="news_card wide_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog_music_techo.jpg" alt="Technology and music" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officia, sequi?</p>
          </div>
        </div>
        <div class="news_card card_2 narrow_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog-post1.jpg" alt="Taking it back to the old school" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt, dicta.</p>
          </div>
        </div>
        <div class="news_card card_3 narrow_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog-post3.jpg" alt="While my guitar gently weeps" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste, possimus!</p>
          </div>
        </div>
        <div class="news_card card_4 narrow_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog-post4.jpg" alt="It just soudns better" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto, animi!</p>
          </div>
        </div>
        <div class="news_card wide_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog_flavor_rock.jpg" alt="The flavor of rock" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Obcaecati, alias.</p>
          </div>
        </div>
        <div class="news_card card_6 narrow_card">
          <div class="news_card_image_container">
            <img src="@/assets/images/blog-post2.jpg" alt="Sharing the stage with a Legend" />
          </div>

          <div class="news_card_text_container">
            <h3>Titolo</h3>
            <p class="small_text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque, praesentium.</p>
          </div>
        </div>
      </div>

      <!-- bottone "vedi tutte le news" (si ripete due volte) -->
      <div class="view_button">
        <a href="#"><p>VIEW ALL LATEST NEWS</p></a>
      </div>
    </div>

    <div class="play_sample"></div>

    <div class="live_dates"></div>
  </div>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style>
</style>