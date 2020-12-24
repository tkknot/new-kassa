<template>
  <div>
    <h1 class="text-center text-h3  my-12 red accent-3 rounded-lg"><span class="white--text">下記説明をよくお読みください</span></h1>

    <v-container class="mb-10">
      <v-row>
        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card height="300">
            <v-card-title >
              <span class="font-weight-bold"
                >次のような状態にある方は、かっさの使用ができません</span
              >
            </v-card-title>
            <ul class="ml-3">
              <li>発熱時、あるいは発熱性の感染症や伝染病の方</li>
              <li>出血傾向にある方、あるいは血小板の少ない方</li>
              <li>白血病の方</li>
              <li>出血性疾患（吐血、喀血、脳出血直後など）の方</li>
              <li>重症の内臓疾患（心臓弁膜症、腎炎など）の方</li>
              <li>潰瘍性疾患（胃潰瘍、十二指腸潰瘍など）の方</li>
              <li>
                癌の手術後の手術部位、あるいは癌の部位<br />
                （癌のある部位でなければ施術は可能です）
              </li>
              <li>妊娠中の方</li>
            </ul>
          </v-card>
        </v-col>
        <v-col cols="12" xl="6" lg="6" md="6" sm="6">
          <v-card height="300">
            <v-card-title>
              <span class="font-weight-bold">
                次のような状態にある方は「ご本人同意」のもと、<br />かっさの使用が可能です
              </span>
            </v-card-title>
            <ul class="ml-3">
              <li>手術後約2ヶ月（個人差あり。体力が回復してから）</li>
              <li>外傷部位のある方（傷、骨折、脱臼時の該当部位付近）</li>
              <li>生理中の方（出血量が増える可能性あり）</li>
              <li>皮膚が炎症を起こしている方</li>
              <li>動脈硬化の方</li>
              <li>静脈瘤がある場所</li>
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
