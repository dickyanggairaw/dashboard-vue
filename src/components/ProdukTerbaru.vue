<template>
  <div class="container margin-container">
      <h4>Promo Terbaru</h4>
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
                    url: "https://kozii.id/img/projects2/2021/06/10/8MXACaJ4QnSwP3z2ykOqI8PmwiuI9yv0.jpg",
                    name: "Eightin Hotel Jakarta"
                },
                {
                    url: "https://kozii.id/img/projects2/2021/06/04/kosPStgdCeeGso1euWvV5Lqaopo9sT4K.jpeg",
                    name: "Hotel Ibis Jakarta"
                },
                {
                    url: "https://kozii.id/img/projects2/2021/06/04/kosPStgdCeeGso1euWvV5Lqaopo9sT4K.jpeg",
                    name: "Hotel Ibis Jakarta"
                },
                {
                    url: "https://kozii.id/img/projects2/2021/06/04/kosPStgdCeeGso1euWvV5Lqaopo9sT4K.jpeg",
                    name: "Hotel Ibis Jakarta"
                },
                {
                    url: "https://kozii.id/img/projects2/2021/06/04/kosPStgdCeeGso1euWvV5Lqaopo9sT4K.jpeg",
                    name: "Hotel Ibis Jakarta"
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