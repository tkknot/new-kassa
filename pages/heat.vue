<template>
  <div>
    <h1
      class="text-center text-xl-h3 text-lg-h3 text-md-h3 text-sm-h3 text-h4 my-12"
    >
      温かっさトリートメント
    </h1>

    <v-container class="my-10">
      <v-row>
        <v-col cols="12" xl="5" lg="5" class="mx-auto">
          <v-img src="/img/L0A0002.jpeg" class="rounded-xl"> </v-img>
        </v-col>

        <v-col cols="12" xl="7" lg="7" class="pl-8">
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            温めたかっさプレートを使って、身体の芯から温めながら全身を施術する、100分のトリートメントです。
          </p>
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            温かいトリートメントですが、女性特有のお悩みにアプローチできる温かっさは、季節を問わず人気です。
          </p>
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            また、かっさプレートの心地良い温かさは、心をゆるめ、<br />
            経絡に沿ってじっくり施術することで、リラクゼーション以上の満足感を得ることが期待できます。
          </p>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">所要時間</h2>
            <div class="text-center">
              <i class="far fa-clock fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">
              約2時間30分 カウンセリング＋施術
            </v-card-text>
          </v-card>
        </v-col>

        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">施術料</h2>
            <div class="text-center">
              <i class="fas fa-wallet fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">10000円 現金のみ</v-card-text>
          </v-card>
        </v-col>

        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">誕生月割引！</h2>
            <div class="text-center">
              <i class="fas fa-birthday-cake fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">2000円引き</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <h1
      class="text-center text-xl-h3 text-lg-h3 text-md-h3 text-sm-h3 text-h4 my-12"
    >
      施術の流れ
    </h1>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card
            max-width="400"
            class="mx-auto"
            elevation="12"
            :height="workCardBreakPoint"
          >
            <v-img
              src="/img/aloma.jpeg"
              max-height="300"
              max-width="400"
            ></v-img>
            <p
              class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8 px-5 pt-2"
            >
              必要事項をシートにご記入いただき、カウンセリングをしていきます。<br />
              その後、五臓に合わせた5種類のメディカルアロマオイルの中から、
              その日の気分に合わせてアロマオイルをお選びいただきます。
            </p>
          </v-card>
        </v-col>

        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card
            max-width="400"
            class="mx-auto"
            elevation="12"
            :height="workCardBreakPoint"
          >
            <v-img
              src="/img/IMG_0075.jpeg"
              max-height="300"
              max-width="400"
            ></v-img>
            <p
              class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8 px-5 pt-2"
            >
              サロンでご用意したウェアに着替えていただきます。
            </p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card
            max-width="400"
            class="mx-auto"
            elevation="12"
            :height="workCardBreakPoint"
          >
            <v-img
              src="/img/workflow2.jpeg"
              max-height="300"
              max-width="400"
            ></v-img>
            <p
              class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8 px-5 pt-2"
            >
              頭頂部から足先まで、約100分の施術を行います。
            </p>
          </v-card>
        </v-col>

        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card
            max-width="400"
            class="mx-auto"
            elevation="12"
            :height="workCardBreakPoint"
          >
            <v-img src="/img/tea.jpeg" max-height="300" max-width="400"></v-img>
            <p
              class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8 px-5 pt-2"
            >
              施術後はかっさとの相乗効果を考えた
              「かっさyuuオリジナル和漢植物ブレンド茶」（いわしや製）
              でおくつろぎください。
            </p>
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
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 260;
        default:
          return 300;
      }
    },
    workCardBreakPoint() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 380;
        default:
          return 500;
      }
    }
  }
};
</script>
