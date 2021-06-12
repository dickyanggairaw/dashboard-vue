<template>
  <div class="container margin-container">
      <h4>8 Alasan Kenapa Bergabung di KOZII</h4>
      <VueSlickCarousel :arrows="true" :dots="true" :infinite="false" :slidesToShow="4">
      <div v-for="(image, i) in images" :key="i">
          <img
            :src="image.url"
            class="d-block height-banner"
            alt="..."
          />
          <p>{{image.name}}</p>
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
    data () {
        return {
            images: [
                {
                    url: "https://kozii.id/web/img/properti/kostel1.jpg",
                    name: "Jakarta"
                },
                {
                    url: "https://kozii.id/web/img/properti/kostel2.jpg",
                    name: "Semarang"
                },
                {
                    url: "https://kozii.id/web/img/properti/kostel3.jpg",
                    name: "Bali"
                },
                {
                    url: "https://kozii.id/web/img/properti/kostel4.jpg",
                    name: "Bogor"
                },
                {
                    url: "https://kozii.id/web/img/properti/bandung.jpg",
                    name: "Bandung"
                },
                {
                    url: "https://kozii.id/web/img/properti/seminyak.jpg",
                    name: "Seminyak"
                },
                {
                    url: "https://kozii.id/web/img/properti/malang.jpg",
                    name: "Malang"
                }
            ]
        }
    }
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
       height: 250px;
       width:  250px;
       margin: 30px;
   }
</style>