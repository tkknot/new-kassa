<template>
  <div>
        <v-bottom-navigation :value="value" grow color="pink" :height="breakPoint">
          <div class="container">
            <div class="row">
              <div class="col-sm-4 mr-0">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint" class="pt-6 mx-auto">
                  <v-card-text class="text--h7">
                    〒250-0051<br>
                    神奈川県小田原市北ノ窪48-1<br>
                    メゾンメルベーユ102<br>
                    電話番号：080-5880-9076<br>
                    メール：kassa.yuu@gmail.com
                  </v-card-text>
                  <div class="container">
                    <div class="row">
                      <div class="col-4 text-center">
                        <a href="https://www.instagram.com/kassa.yuu/">
                          <i class="fab fa-instagram fa-4x" style="color: #D93177;"></i>
                        </a>
                      </div>
                      <div class="col-4 text-center">
                        <a
                          href="https://ja-jp.facebook.com/pages/category/Health-Beauty/%E3%81%8B%E3%81%A3%E3%81%95-yuu-146418565810698/">
                          <i class="fab fa-facebook-square fa-4x" style="color: #3B5998;"></i>
                        </a>
                      </div>
                      <div class="col-4">
                        <a href="https://ameblo.jp/yuu-kassa/">
                          <p id="Ameba">Ameba</p>
                        </a>
                      </div>
                    </div>
                  </div>
                </v-card>
              </div>
              <div class="col-sm-4">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint" class="pt-6 mx-auto">
                  <v-card-text class="text--h7">
                    COVID-19対策のため、<br>
                    ご予約可能時間を<br>
                    (月)(火)(金)(土)の10:00～15:00(施術開始時間)とさせていただきます。<br>
                    なお、ご連絡は前日19：00までにお願いします。<br>
                    ※ご予約は１日１名様限定となっております。
                  </v-card-text>
                  <v-card-text class="text--h7">
                    ※ご予約はお電話もしくは<br>
                    メールでお問い合わせください。
                  </v-card-text>
                </v-card>
              </div>
              <div class="col-sm-4 col-xs-12">
                <v-card :width="cardWidthBreakPoint" :height="cardBreakPoint"
                  class="d-flex justify-content-center align-items-center mx-auto">
                  <div id="map-box" class="w-75 h-75"></div>
                </v-card>
              </div>
            </div>
          </div>
        </v-bottom-navigation>

    <v-footer  color="black" height="40px" >
      <p class="text-center mb-0 text-h5" id="footer-text">
      ©{{ new Date().getFullYear() }} kassa-yuu
      </p>
    </v-footer>
  </div>
</template>

<style lang="scss" scoped>

  #footer-text {
    width: 100%;
    color: white;
  }

#Ameba {
  height: 60px;
  width: 60px;
  color: white;
  background-color: green;
}

</style>

<script>
//   if (process.client) {
//     function initMap() {
//   const mapBox = document.getElementById("map-box");
//   var map;
//   var salon = {
//     lat: 35.2896889,
//     lng: 139.1335604,
//   };
//   var marker;

//   map = new google.maps.Map(mapBox, {
//     center: salon,
//     zoom: 15,
//   });

//   var marker = new google.maps.Marker({
//     position: salon,
//     map: map,
//     animation: google.maps.Animation.DROP, 
//   });
// }
  // }

export default {
  data(){
    return {
      value: 1
    }
  },
    computed: {
    breakPoint() {
      let bP = this.$vuetify.breakpoint.name;
      if (bP === "xs") {
        return "1000px";
      } else if (bP === "sm") {
        return "500px";
      } else {
        return "500px";
      }
    },
    cardBreakPoint() {
      let bP = this.$vuetify.breakpoint.name;
      if (bP === "xs") {
        return "300px";
      } else if (bP === "sm") {
        return "400px";
      } else {
        return "400px";
      }
    },
    cardWidthBreakPoint() {
      let bP = this.$vuetify.breakpoint.name;
      if (bP === "xs") {
        return "400px";
      } else if (bP === "sm") {
        return "216px";
      } else {
        return "370px";
      }
    },
  },

}

</script>