<template>
    <div class="container-fluid bg-light">
        <Logo/>
        <PromoMenarik/>
        <ProdukTerbaru/>
        <Produk/>
        <City/>
        <Hotel/>
        <Apartemen/>
        <div class="container">
          <img src="https://kozii.id/web/img/v-office-banner.jpeg" alt="">
        </div>
        <Subscribe/>
        <Footer/>
    </div>
</template>

<script>
// @ is an alias to /src
import Logo from '../components/Logo'
import PromoMenarik from '../components/PromoMenarik'
import ProdukTerbaru from '../components/ProdukTerbaru'
import Produk from '../components/Produk'
import City from '../components/City'
import Apartemen from '../components/Apartemen'
import Subscribe from '../components/Subscribe'
import Footer from '../components/Footer'
import Hotel from '../components/Hotel'
export default {
  name: 'Home',
  components: {
    Logo,
    PromoMenarik,
    ProdukTerbaru,
    Produk,
    City,
    Apartemen,
    Subscribe,
    Footer,
    Hotel
  }
}
</script>

<style scoped>
   .container-fluid {
      padding-top: 20px;
      padding-bottom: 40px;
      padding-left: auto;
      padding-right: auto;
   }
   /* .container {
     text-align: left;
   } */
</style>