<template>
  <div>
    <v-container class="my-10">
      <v-row>
        <v-col cols="12" xl="12" lg="12" class="pl-8">
          <h1
            class="text-center text-xl-h3 text-lg-h3 text-md-h3 text-sm-h3 text-h4 my-12"
          >
            スペシャルコース
          </h1>

          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            温かっさ＋フェイスかっさ＋ハンドトリートメントのスペシャルコースです。
          </p>
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            全身のかっさはトータルバランスで診立てる、 とても価値のあるものです。
          </p>
          <p class="text-xl-h6 text-lg-h6 text-md-h6 text-sm-h6 text-h8">
            頑張る自分のご褒美に、ぜひご利用ください。
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
              約3時間 カウンセリング＋施術
            </v-card-text>
          </v-card>
        </v-col>

        <v-col cols="12" xl="4" lg="4" md="4" sm="4">
          <v-card color="white" elevation="8" :height="threeCardBreakPoint">
            <h2 class="text-center py-7">施術料</h2>
            <div class="text-center">
              <i class="fas fa-wallet fa-5x pb-3"></i>
            </div>
            <v-card-text class="text-center text-h6">18000円 現金のみ</v-card-text>
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
  </div>
</template>
