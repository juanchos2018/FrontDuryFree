<template>
  <div class="hero is-medium is-bold">
    <div class="">
      <div class="">
       <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1000"
      img-height="380"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide       
        img-src="portada2.png"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="portada1.jpg">
    
          <!--     <h1>Hello world!</h1> -->
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="portada3.jpg"></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <template #img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="portada4.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>      
    </b-carousel>
      </div>
    </div>
  
    
  </div>
</template>



<script>
import Vue from 'vue'
import Promo from '../promo/Promo'
export default {

   name: 'VmHeader',
   components: {
      Promo,    
    
    },
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
}
</script>


<style lang="scss" scoped>
    .hero {
      background: rgb(81, 186, 252);
    }
    h1, h2 {
      color: #fff;
    }
</style>