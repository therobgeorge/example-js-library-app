<template>
  <div class="slides">
    <h1>Rad Women</h1>
    <VueSlickCarousel v-bind="settings">
      <img
        src="https://cdn.vox-cdn.com/thumbor/_fpCSj9i7hG2kGlh2yWuhokAD9I=/1400x1400/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/21763517/USAvNED_20190707182726_5290_001.jpg"
        alt="Rose Lavelle"
      />
      <img src="https://www.ocregister.com/wp-content/uploads/2021/06/AP21162088701648.jpg" alt="Sam Mewis" />
      <img src="https://morningstaronline.co.uk/sites/default/files/PA-59235059.jpg" alt="Chloe Kelley" />
      <img src="https://upload.wikimedia.org/wikipedia/en/0/0a/Taylor_Swift_-_Evermore.png" alt="" />
      <img
        src="https://64.media.tumblr.com/64592f93548617e226d28fd30716227e/6d924fa9e38abe5b-30/s1280x1920/555b63e9db8ecc9757dc9c952be3f2fa49d8d2cb.jpg"
        alt=""
      />
    </VueSlickCarousel>
  </div>
</template>
<style>
.slides {
  max-width: 600px;
  margin-left: 25%;
}
</style>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  data: function () {
    return {
      settings: {
        arrow: true,
        dots: true,
        fade: true,
        infinite: true,
        speed: 500,
        slidesToShow: 1,
        slidesToScroll: 1,
      },
    };
  },
  name: "MyComponent",
  components: { VueSlickCarousel },
};
</script>
