<template>
  <div class="main">
    <div class="brake">
      <!-- sezione di testo (si ripete 3 volte nel codice) -->
      <div class="main_text_section">
        <!-- linea rossa -->
        <div class="brake_red_line"></div>

        <h2>Music Is Life</h2>
        <div class="div_line"></div>

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
        <div class="div_line"></div>

        <p class="small_text">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos
          ea at explicabo adipisci doloremque quae non quam ab, vitae nisi
          porro, nihil quisquam id vel provident suscipit architecto dolores
          perspiciatis!
        </p>
      </div>

      <!-- contenitore delle news -->
      <div class="news_container">
        <div class="news_card card_1 wide_card">
          <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>Technology and music</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog_music_techo.jpg"
              alt="Technology and music"
            />
          </div>

          <div class="news_card_text_container">
            <h3>Technology and music</h3>
            <p class="small_text">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officia,
              sequi?
            </p>
          </div>
        </div>
        <div class="news_card card_2 narrow_card">
           <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>Taking it back to the old school</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog-post1.jpg"
              alt="Taking it back to the old school"
            />
          </div>

          <div class="news_card_text_container">
            <h3>Taking it back to the old school</h3>
            <p class="small_text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt,
              dicta.
            </p>
          </div>
        </div>
        <div class="news_card card_3 narrow_card">
          <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>While my guitar gently weeps</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog-post3.jpg"
              alt="While my guitar gently weeps"
            />
          </div>

          <div class="news_card_text_container">
            <h3>While my guitar gently weeps</h3>
            <p class="small_text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste,
              possimus!
            </p>
          </div>
        </div>
        <div class="news_card card_4 narrow_card">
          <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>It just sounds better</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog-post4.jpg"
              alt="It just soudns better"
            />
          </div>

          <div class="news_card_text_container">
            <h3>It just sounds better</h3>
            <p class="small_text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto,
              animi!
            </p>
          </div>
        </div>
        <div class="news_card card_5 wide_card">
          <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>The flavor of rock</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog_flavor_rock.jpg"
              alt="The flavor of rock"
            />
          </div>

          <div class="news_card_text_container">
            <h3>The flavor of rock</h3>
            <p class="small_text">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              Obcaecati, alias.
            </p>
          </div>
        </div>
        <div class="news_card card_6 narrow_card">
          <!-- il link compare quando la card è in hover -->
          <div class="hover_link">
            <a href="#"><p>Sharing the stage with a Legend</p></a>
          </div>

          <div class="news_card_image_container">
            <img
              src="@/assets/images/blog-post2.jpg"
              alt="Sharing the stage with a Legend"
            />
          </div>

          <div class="news_card_text_container">
            <h3>Sharing the stage with a Legend</h3>
            <p class="small_text">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit.
              Doloremque, praesentium.
            </p>
          </div>
        </div>
      </div>

      <!-- bottone "vedi tutte le news" (si ripete due volte) -->
      <div class="view_button">
        <a href="#"><p>VIEW ALL LATEST NEWS</p></a>
      </div>
    </div>

    <div class="play_sample">
      <div class="quote_container">
        <p class="big_text">
          <em>
            "I just ilstened to it adn said to myself, "Man, I really love this
            album." Still, today, it just sounds so fresh. It sounds full of
            ideas. These guys knew what they were doing. THey're good. And
            they're inventive. I havent't heard aniything this yeat that is that
            inventive. I don't really ecpect to."
          </em>
        </p>

        <div class="play_button">
          <a href="#">
            <i class="fas fa-play"></i>
          </a>
        </div>
      </div>
    </div>

    <div class="live_dates">
      <div class="main_text_section">

        <h2>Live dates</h2>
        <div class="div_line"></div>

        <p class="small_text">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos
          ea at explicabo adipisci doloremque quae non quam ab, vitae nisi
          porro, nihil quisquam id vel provident suscipit architecto dolores
          perspiciatis!
        </p>
      </div>

      <div class="live_dates_list">
        <ul>
          <li></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style>
</style>