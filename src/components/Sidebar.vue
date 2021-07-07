<template>
  <div>
    <v-card> 
    <v-navigation-drawer app permanent expand-on-hover >
      <v-list>
        <v-list-item class="px-2">
          <v-list-item-avatar style="height: 100px;min-width: 100px;width: 100px; margin-left:50px;">
            <v-img
              src="https://professorwerner.org/wp-content/uploads/2016/11/richard_werner_speech_4_s.jpg"
            ></v-img>
          </v-list-item-avatar>
        </v-list-item>
        <v-list-item link>
            <v-list-item-content>
              <v-list-item-title class="text-h6">
                Osundahunsi, Oluwatooyin Faramade
              </v-list-item-title>
              <v-list-item-subtitle>Professor, Federal University of Technology, Akure.</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list nav dense>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home-city</v-icon>
          </v-list-item-icon>
          <v-list-item-title @click="home" >Home</v-list-item-title>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-account-multiple</v-icon>
          </v-list-item-icon>
          <v-list-item-title @click="projectlink">Projects</v-list-item-title>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-star</v-icon>
          </v-list-item-icon>
          <v-list-item-title @click="gallerylink">Gallery</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    </v-card>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data: () => ({
    collapseOnScroll: true,
  }),
  methods:{
    gallerylink: function(){
      this.$router.push({ path: '/Gallery'})
    },
    home: function(){
      this.$router.push({ path: '/' })
    },
    projectlink: function(){
      this.$router.push({ path: '/Projects' })
    }
      
  }
};
</script>

<style scoped>

</style>