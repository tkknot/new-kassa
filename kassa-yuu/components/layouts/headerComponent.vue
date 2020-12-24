<template>
  <div>
    <v-navigation-drawer
      app
      v-model="drawer"
      temporary
      color="rgba(250, 221, 205, 1)"
    >
      <v-list>
        <v-list-item nuxt to="/" class="my-4">Home</v-list-item>
        <v-list-item nuxt to="/therapist" class="my-4">セラピスト</v-list-item>
        <v-list-item nuxt to="/heat" class="my-4">温かっさ</v-list-item>
        <v-list-item nuxt to="/seminar" class="my-4">セルフかっさ</v-list-item>
        <v-list-item nuxt to="/caution" class="my-4">注意事項</v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar hide-on-scroll height="340" color="rgba(250, 221, 205, 1);">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-container fluid>
        <v-row no-gutters>
          <v-col cols="5">
            <v-img src="/img/logo-new.jpg" height="340"></v-img>
          </v-col>
          <v-col cols="7" id="ccbox">
            <span id="catchcopy" class="text-h2 text-center">
              one step ahead in relaxation
            </span>
          </v-col>
        </v-row>
      </v-container>
    </v-app-bar>
  </div>
</template>

<style lang="scss" scoped>
#ccbox {
  position: relative;
}

#catchcopy {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateY(-50%) translateX(-50%);
  width: 100%;
  color: white;
  font-family: "Noto Serif JP", serif;
}

.v-expansion-panel-content__wrap {
  & > a {
    padding: 0;
    width: 100%;
  }
}
</style>

<script>
export default {
  data() {
    return {
      drawer: null
    };
  }
};
</script>
