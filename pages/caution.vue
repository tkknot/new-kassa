<template>
  <div>
    <h1
      class="text-center text-xl-h3 text-lg-h3 text-md-h3 text-sm-h3 text-h4 my-12"
    >
      下記説明を<br id="br" />よくお読みください
    </h1>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <!-- caution left -->
          <v-card :height="cautionCardHeight">
            <v-card-title>
              <span class="font-weight-bold"
                >次のような状態にある方は、<br
                  id="br"
                />かっさの使用ができません</span
              >
            </v-card-title>

            <ul class="ml-3">
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                発熱時、あるいは発熱性の感染症や伝染病の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                出血傾向にある方、あるいは血小板の少ない方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                白血病の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                出血性疾患（吐血、喀血、脳出血直後など）の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                重症の内臓疾患（心臓弁膜症、腎炎など）の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                潰瘍性疾患（胃潰瘍、十二指腸潰瘍など）の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                癌の手術後の手術部位、あるいは癌の部位<br />
                （癌のある部位でなければ施術は可能です）
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                妊娠中の方
              </li>
            </ul>
          </v-card>
        </v-col>

        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card :height="cautionCardHeight">
            <!-- caution right -->
            <v-card-title>
              <span class="font-weight-bold">
                次のような状態にある方は<br
                  id="br"
                />「ご本人同意」のもと、<br />かっさの使用が可能です
              </span>
            </v-card-title>

            <ul class="ml-3">
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                手術後約2ヶ月（個人差あり。体力が回復してから）
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                外傷部位のある方（傷、骨折、脱臼時の該当部位付近）
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                生理中の方（出血量が増える可能性あり）
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                皮膚が炎症を起こしている方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                動脈硬化の方
              </li>
              <li
                class=" text-xl-h7 text-lg-h7 text-md-h7 text-sm-h7 text-h10 my-12"
              >
                静脈瘤がある場所
              </li>
            </ul>

            <p class="text-h6 ml-3 my-3">
              ※持病のある方は、かかりつけの医師にご相談ください
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
    cautionCardHeight: function() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 780;
        default:
          return 700;
      }
    }
  }
};
</script>
