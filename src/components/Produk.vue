<template>
  <div class="container margin-container">
      <h4>Produk</h4>
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
                    url: "https://kozii.id/img/hot/properti.jpg",
                    name: "Properti"
                },
                {
                    url: "https://kozii.id/img/hot/fashion.jpg",
                    name: "Fashion"
                },
                {
                    url: "https://kozii.id/img/hot/fnb.jpg",
                    name: "Makanan & Minuman"
                },
                {
                    url: "https://kozii.id/img/hot/beauty.jpg",
                    name: "Kesehatan"
                },
                {
                    url: "https://kozii.id/img/hot/healthy.jpg",
                    name: "Kesehatan"
                },
                {
                    url: "https://kozii.id/img/hot/fnb.jpg",
                    name: "UMKM"
                },
                {
                    url: "https://kozii.id/img/hot/finance.jpg",
                    name: "Finance"
                },
                {
                    url: "https://kozii.id/img/hot/jasa.jpg",
                    name: "Jasa"
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
       height: 150px;
       width:  250px;
       margin: 30px;
   }
</style>