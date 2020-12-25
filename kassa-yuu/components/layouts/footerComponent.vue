<template>
  <div>
    <v-bottom-navigation :value="value" grow color="pink" :height="breakPoint">
      <v-container>
        <v-row>
          <v-col cols="12" xl="4" lg="4" md="4" sm="4">
            <v-card
              :width="cardWidthBreakPoint"
              :height="cardBreakPoint"
              class="pt-6 mx-auto"
            >
              <v-card-text class="text--h7">
                〒250-0051<br />
                神奈川県小田原市北ノ窪48-1<br />
                メゾンメルベーユ102<br />
                電話番号：080-5880-9076<br />
                メール：kassa.yuu@gmail.com
              </v-card-text>
              <v-container>
                <v-row>
                  <v-col cols="4" class="text-center">
                    <a href="https://www.instagram.com/kassa.yuu/">
                      <i
                        class="fab fa-instagram fa-4x"
                        style="color: #D93177;"
                      ></i>
                    </a>
                  </v-col>
                  <v-col cols="4" class="text-center">
                    <a
                      href="https://ja-jp.facebook.com/pages/category/Health-Beauty/%E3%81%8B%E3%81%A3%E3%81%95-yuu-146418565810698/"
                    >
                      <i
                        class="fab fa-facebook-square fa-4x"
                        style="color: #3B5998;"
                      ></i>
                    </a>
                  </v-col>
                  <v-col cols="4" class="text-center">
                    <a href="https://ameblo.jp/yuu-kassa/">
                      <p id="Ameba">Ameba</p>
                    </a>
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-col>

          <v-col cols="12" xl="4" lg="4" md="4" sm="4">
            <v-card
              :width="cardWidthBreakPoint"
              :height="cardBreakPoint"
              class="pt-6 mx-auto"
            >
              <v-card-text class="text--h7">
                COVID-19対策のため、<br />
                ご予約可能時間を<br />
                (月)(火)(金)(土)の10:00～15:00(施術開始時間)とさせていただきます。<br />
                なお、ご連絡は前日19：00までにお願いします。<br />
                ※ご予約は１日１名様限定となっております。
              </v-card-text>
              <v-card-text class="text--h7">
                ※ご予約はお電話もしくは<br />
                メールでお問い合わせください。
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="12" xl="4" lg="4" md="4" sm="4">
            <v-card
              :width="cardWidthBreakPoint"
              :height="cardBreakPoint"
              class="d-flex justify-content-center align-items-center mx-auto"
            >
              <GmapMap
                map-type-id="roadmap"
                :center="maplocation"
                :zoom="zoom"
                :style="styleMap"
              >
                <GmapMarker
                  v-for="(m, index) in markers"
                  :key="index"
                  :position="m.position"
                  :clickable="true"
                  :draggable="false"
                  :icon="m.pinicon"
                  @click="onClickMarker(index, m)"
                />
              </GmapMap>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-bottom-navigation>

    <v-footer color="black" height="40px">
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
export default {
  data() {
    return {
      value: 1,
      maplocation: { lng: 139.1335604, lat: 35.2896889 },
      zoom: 15,
      styleMap: {
        width: "75%",
        height: "75%",
        margin: "auto"
      },
      markers: [
        {
          position: { lng: 139.1335604, lat: 35.2896889 }
        }
      ]
    };
  },
  computed: {
    breakPoint() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 1000;
        default:
          return 500
      }
    },
    cardBreakPoint() {
      let bP = this.$vuetify.breakpoint.name;
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 300;
        default:
          return 500
      }
    },
    cardWidthBreakPoint() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 400;
        case "sm":
          return 220;
        default:
          return 370
      }
    }
  }
};
</script>
