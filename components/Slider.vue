<template>
  <div class="slider-div">
    <VueSlickCarousel
      v-bind="settings"
      v-editable="blok">
      <div 
        :key="blok._uid"
        v-for="blok in blok.slides">
        <component :blok="blok" :is="blok.component" class="slider-image"></component>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<style>
  .slider-image img {
    height: auto;
    width: 100%;
  }
  .slider-div {
    padding-top: 0px;
    margin-top: -80px;
  }
  .slick-prev:before {
    color: black;
  }
  .slick-next:before {
    color: black;
  }
</style>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  data(){
    return {
      settings: {
        dots: true,
        slidesToShow: 3
      }
    }
  },
  components: { VueSlickCarousel },
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>