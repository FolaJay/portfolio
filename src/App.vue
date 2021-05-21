<template>
  <v-app>
    <Sidebar />
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
