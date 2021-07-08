<template>
  <v-app>
    <Sidebar/>
    <v-content>
            <v-container fluid>
                <v-row class="fill-height">
                    <v-col>
                        <transition name="fade">
                            <router-view></router-view>
                        </transition>
                    </v-col>
                </v-row>
            </v-container>
        </v-content>

  </v-app>
</template>

<script>
import Sidebar from '@/components/Sidebar.vue'
export default {
  name: 'App',

  components: {
    Sidebar,
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merienda&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

span{
  color: rgb(0 0 0 / 70%);
}
body {
  font-family: 'Roboto', sans-serif !important;
  
}
</style>
