<template>
  <v-app app>
    <headerComponent />

    <v-main>
      <v-container>
        <!-- <nuxt /> -->
      </v-container>
    </v-main>

    <footerComponent />
  </v-app>
</template>

<style lang="scss" scoped>
h1 #footer-letters {
  font-family: "HG正楷書体-PRO", "cursive";
}

h2 {
  font-family: "Noto Sans JP", sans-serif;
}

p {
  font-family: "Noto Serif JP", serif;
}

li {
  font-family: "Noto Serif JP", serif;
}
</style>

<script>
import headerComponent from '~/components/layouts/headerComponent.vue'
import footerComponent from '~/components/layouts/footerComponent.vue'

export default {
  components: {
    headerComponent,
    footerComponent,
  }
}
</script>