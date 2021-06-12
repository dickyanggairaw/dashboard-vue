<template>
  <div class="container margin-container">
      <h4>Promo Menarik</h4>
      <VueSlickCarousel :arrows="true" :dots="true" :infinite="false" :slidesToShow="3">
      <div>
          <img
            src="https://kozii.id/img/promo/2021/06/10/KIG5YAf19VODfRJhUq9WmiWq2xBFNI6h.jpg"
            class="d-block height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/promo/2021/06/11/0C0avH7fIn5SzSZAROu2ABrE37N4JLRP.jpg"
            class="d-block height-banner"
            alt="..."
          />
        </div>
        <div>
          <img
            src="https://kozii.id/img/promo/2021/01/31/zMLSGf5AgILjWRkWz3rIQ3mc98UfqZwO-baru.jpg"
            class="d-block height-banner"
            alt="..."
          />
        </div>
    </VueSlickCarousel>
      <div class="row">
      </div>
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
    .margin-container {
        background-color: white;
        border-radius: 10px;
        padding: 20px;
        margin-bottom: 10px;
    }
    .slick-next::before {
     color: black;
   }

   .slick-prev::before{
     color: black;
   }
   h4 {
       text-align: left; 
   }
   img {
       height: 350px;
       width:  350px;
       margin: 30px;
   }
</style>