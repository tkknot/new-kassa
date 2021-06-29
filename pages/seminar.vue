<template>
  <div>
    <h1
      class="text-center text-xl-h3 text-lg-h3 text-md-h3 text-sm-h3 text-h4 my-12"
    >
      自宅でできる<br id="br" />セルフかっさセミナー
    </h1>

    <p
      class="text-center text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8 red--text accent-2"
    >
      ※かっさプレートが品薄のため、<br id="br" />現在は受付を終了しています。
    </p>

    <v-container class="my-10">
      <v-row>
        <v-col cols="12" xl="5" lg="5" class="mx-auto">
          <v-img src="img/J6A0109.jpeg" class="rounded-xl"></v-img>
        </v-col>

        <v-col cols="12" xl="7" lg="7" class="pl-8">
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            日頃のセルフケアとして、ボディかっさマッサージを習得していただけるセミナーです。<br />
            病院へ行くほどではない身体の不調の改善法、スリミング効果のあるマッサージの仕方をお伝えします。
          </p>

          <ul>
            <li class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
              温かっさトリートメントを受けられた方は、サロンにてマンツーマンレッスン可能です。
            </li>
            <li class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
              多人数でのセミナーのご依頼も承ります。（別途交通費・出張料がかかります。）お気軽にご相談ください。
            </li>
            <li class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
              服装は首周りのスッキリとした上衣、下衣はパンツスタイルでお願い致します
            </li>
          </ul>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">受講時間</h2>
            <div class="text-center">
              <i class="far fa-clock fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">約2時間</v-card-text>
          </v-card>
        </v-col>

        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">受講料</h2>
            <div class="text-center">
              <i class="fas fa-wallet fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">13000円 現金のみ</v-card-text>
          </v-card>
        </v-col>

        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">その他</h2>
            <div class="text-center">
              <i class="fas fa-gift fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-h7"
              >金額にプレート代及びテキスト代を含んでおります。</v-card-text
            >
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  computed: {
    threeCardBreakPoint() {
      let bP = this.$vuetify.breakpoint.name;
      if (bP === "xs") {
        return "260px";
      } else if (bP === "sm") {
        return "300px";
      } else {
        return "300px";
      }
    }
  }
};
</script>
