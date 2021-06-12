<template>
  <div class="container banner">
    <VueSlickCarousel :arrows="true" :dots="true" :autoplay="true">
      <div>
          <img
            src="https://kozii.id/img/sliders/2021/06/05/jP1vvGUID2QjBS4hc8r0UC4LZSDFhY8g.jpg"
            class="d-block w-100 h-50 height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/sliders/2021/06/05/Tj70KiA7zm6UTvD62nCRyD4C9bqL8xnS.jpg"
            class="d-block w-100 height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/sliders/2021/06/08/3qbScJYSj2wTL9NM6Y2gmnV7bZlKZN3F.jpg"
            class="d-block w-100 height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/sliders/2021/06/08/uQoPUdVFzwLzh6FnIAwLVw8HMv4Kyapz.jpg"
            class="d-block w-100 height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/sliders/2021/06/04/ofJpL74TwQLpNgR1aTiXfcZslxlPWWyv.jpg"
            className="d-block w-75 height-banner"
            alt="..."
          />
        </div>
    </VueSlickCarousel>
  </div>
</template>
 
<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
 
  export default {
    name: 'MyComponent',
    components: { VueSlickCarousel },
  }
</script>

<style scoped>
    .banner {
        margin-bottom: 50px;
    }
</style>