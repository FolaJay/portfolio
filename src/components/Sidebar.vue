<template>
  <div>
    <v-navigation-drawer app floating class="teal lighten-2">
      <v-list>
        <v-list-item class="px-2">
          <v-list-item-avatar style="height: 100px;min-width: 100px;width: 100px; margin-left:50px;">
            <v-img
              src="https://professorwerner.org/wp-content/uploads/2016/11/richard_werner_speech_4_s.jpg"
            ></v-img>
          </v-list-item-avatar>
        </v-list-item>
        

        <v-list-item link class="v-list-item v-list-item--link theme--light">
          <v-list-item-content>
            <v-list-item-title class="title"> Richard A. William </v-list-item-title>
            <v-list-item-subtitle class="v-list-item__subtitle"
              >DPhil (Oxon) | Linacre College, University of
              Oxford</v-list-item-subtitle
            >
          </v-list-item-content>
        </v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list nav dense>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home-city</v-icon>
          </v-list-item-icon>
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-account-multiple</v-icon>
          </v-list-item-icon>
          <v-list-item-title>Projects</v-list-item-title>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-star</v-icon>
          </v-list-item-icon>
          <v-list-item-title>Gallery</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data: () => ({
    collapseOnScroll: true,
  }),
};
</script>

<style scoped>
.theme--light.v-list-item:not(.v-list-item--active):not(.v-list-item--disabled) {
  color: #fff !important;
}
.theme--light.v-list-item .v-list-item__subtitle,
.theme--light.v-list-item .v-list-item__action-text {
  color: #fff;
}
.title {
  font-weight: 300;
  color: #fff;
  margin: 20px 0 10px 0;
}
.v-list-item__title,
.v-list-item__subtitle {
  white-space: normal !important;
}
</style>