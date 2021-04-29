<template>
    <div class="container">
        <div class="section-padding container-fluid bg-image bg-position-cc text-center overlay-light90" style="background-image:url(assets/img/bg/bg_5.jpg)">
        <div class="container-lg">
            <div class="mb-5 text-center">
                <h2 class="page-title font-900 text-uppercase mb-2">Nuestras Categorías</h2>
                <a href="#" class="section__more-link text-center text-uppercase">Ver Más <svg class="icon--tail-right" width="16px" height="16px" viewBox="0 0 24 24" role="presentation"><path fill="currentColor" d="M22.707 11.293L15 3.586 13.586 5l6 6H2c-.553 0-1 .448-1 1s.447 1 1 1h17.586l-6 6L15 20.414l7.707-7.707c.391-.391.391-1.023 0-1.414z"></path></svg></a>
            </div>
        </div>
    </div>
    <div>
        <VueSlickCarousel  :dots="true"   :focusOnSelect="true"
            :infinite="true"
            :speed="500"
            :slidesToShow="3"
            :slidesToScroll="1"
            :touchThreshold="5"           
            :autoplay="true">
        <div  style="margin-left:10px">
          <b-img src="categoria1.png"   style="margin-left:5px;padding:5px" ></b-img>
          <br>
          <center> <h6 class="text-uppercase">PERFUMERIA</h6></center>
         
        </div>
        <div style="margin-left:10px">
              <b-img src="categoria2.png"     ></b-img>
              <br>
               <center> <h6 class="text-uppercase">LICORES</h6></center>
        </div>
        <div>
              <b-img src="categoria3.jpg"    ></b-img>
              <br>
              <center> <h6 class="text-uppercase">RELOJES</h6></center>
        </div>
        <div>
              <b-img src="categoria4.jpg"     ></b-img>
              <br>
              <center> <h6 class="text-uppercase">ACCESORIOS</h6></center>
        </div>
        </VueSlickCarousel>
  </div>
    </div>
</template>
<script>
 import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
 import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name: 'categoria',
    components: { VueSlickCarousel },
    created(){
        return{
           
        }
    }
}
</script>

<style lang="scss" scoped>

</style>