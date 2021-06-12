<template>
  <div class="container" style="margin-top: 20px;">
      <div class="row">
          <div class="col-6">
              <div class="row">
                  <div class="col-3">
                      <img src="https://kozii.id/web/img/logo-footer.png" width="100" height="40" alt="">
                  </div>
                  <div class="col-5">
                      <img src="https://kozii.id/img/icon/twitter.png" width="25" height="25" alt="">
                      <img src="https://kozii.id/img/icon/whatsapp.png" width="25" height="25" alt="">
                      <img src="https://kozii.id/img/icon/linkedin.png" width="25" height="25" alt="">
                      <img src="https://kozii.id/img/icon/facebook.png" width="25" height="25" alt="">
                      <img src="https://kozii.id/img/icon/instagram.png" width="25" height="25" alt="">
                  </div>
              </div>
                <div class="progress" style="height: 1px;">
                    <div class="progress-bar" role="progressbar" style="width: 100%;" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
                </div>
                <p>Asosiasi & Developer</p>
                <div class="row">
                    <div class="col-2" v-for="(developer, i) in developers" :key="i">
                        <img :src="developer" width="50" alt="">
                    </div>
                </div>
                <p>Bank</p>
                <div class="row">
                    <div class="col-2" v-for="(bank, i) in banks" :key="i">
                        <img :src="bank" width="50" alt="">
                    </div>
                </div>
                <p>Media</p>
                <div class="row">
                    <div class="col-2" v-for="(media, i) in medias" :key="i">
                        <img :src="media" width="50" alt="">
                    </div>
                </div>
          </div>
          <div class="col-6">
                <div class="row">
                    <div class="col-4">
                        <h5>Tentang Kozi</h5>
                        <a href="">Tentang Kami</a><br>
                        <a href="">Team</a><br>
                        <a href="">Pusat Bantuan</a><br>
                        <a href="">Hubungi Kami</a><br>
                        <a href="">Lokasi</a>
                    </div>
                    <div class="col-3">
                        <h5>Lainnya</h5>
                        <a href="">Privacy</a><br>
                        <a href="">Syarat & ketentuan berlaku</a><br>
                    </div>
                    <div class="col-5">
                        <h5>Download Kozi App</h5>
                        <img src="https://kozii.id/img/icon/google-play-badge.png" width="200" alt="">
                    </div>
                </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    data () {
        return {
            developers: [
                "https://kozii.id/img/icon/partner/arebi.png",
                "https://kozii.id/img/icon/partner/penta.png",
                "https://kozii.id/img/icon/partner/benhokk.png",
                "https://kozii.id/img/icon/partner/mahameru.png",
                "https://kozii.id/img/icon/partner/ciputra.png",
                "https://kozii.id/img/icon/partner/sis.png",
                "https://kozii.id/img/icon/partner/puri.png",
                "https://kozii.id/img/icon/partner/kalmar.png",
                "https://kozii.id/img/icon/partner/pp.png",
                "https://kozii.id/img/icon/partner/agung-podomoro.png",
                "https://kozii.id/img/icon/partner/logo-transpark.png"
            ],
            banks: [
                "https://kozii.id/img/icon/partner/smf.png",
                "https://kozii.id/img/icon/partner/bjb_syariah.png",
                "https://kozii.id/img/icon/partner/panin-syariah.jpg"
            ],
            medias: [
                "https://kozii.id/img/icon/partner/logo-harian.png",
                "https://kozii.id/img/icon/partner/logo-mahaka.png"
            ]
        }
    }
}
</script>

<style>
    a {
        text-decoration: none;
        color: black;
    }
</style>