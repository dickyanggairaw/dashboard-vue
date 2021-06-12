<template>
  <div class="container margin-container">
      <h4>Hot Deal Hotel</h4>
      <p>Piihan hotel dengan harga menarik di sekitar Anda</p>
      <VueSlickCarousel :arrows="true" :dots="true" :infinite="false" :slidesToShow="4">
      <!-- <div v-for="(image, i) in images" :key="i">
          <img
            :src="image.url"
            class="d-block height-banner img-hover-zoom img-hover-zoom--colorize"
            alt="..."
          />
          <h4 class="banner-text">{{image.name}}</h4>
        </div> -->
        <div class=" mb-4 team-area" v-for="(image, i) in images" :key="i">
            <div class="single-team">
            <img v-bind:src="image.url" class="w-100 item-cart-2" alt="...">
            <div class="card-body body-style team-text">
                <h5 className="mb-0">{{image.name}}</h5>
            </div>
            </div>
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
        object-fit: cover;
        object-position: center;
   }
   .banner-text {
        position: absolute;
        top: 220px;
        left: 100px;
        font-size: 20px;
        color: white;
        }
    .single-team {
  position: relative;
  display: flex;
  align-items: flex-end;
  transition: 0.6s ease-out;
  padding: 25px;
}
.single-team:hover {
  transform: scale(1.1);
}
.single-team:hover:before {
  opacity: 1;
}
.single-team .team-text {
  position: relative;
  z-index: 2;
  color: #fff;
  opacity: 0;
  transform: translateY(60px);
  transition: 1s;
}
.single-team:hover .team-text {
  opacity: 1;
  transform: translateY(0);
  transform: translateX(-200px);
}
.single-team:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  display: block;
  width: 105%;
  height: 100%;
  background: linear-gradient(to top, rgb(71, 71, 71), transparent);
  z-index: 2;
  transition: 0.5s;
  opacity: 0;
}
</style>