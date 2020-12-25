<template>
  <v-app app>
    <headerComponent />

    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>

    <footerComponent />
  </v-app>
</template>

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