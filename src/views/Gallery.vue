<template>
    <v-app>
        <v-container class="section5">
          <h2 class="heading">PHOTO SPEAK</h2>
          <v-row>
              <v-col cols="12" class="text-center custom-btn">
            <v-btn class="red lighten-1 btn">
              <router-link to="/" class="custom-btn-link">
                Back
              </router-link>
            </v-btn>
          </v-col>
            <v-col v-for="n in 18" :key="n" class="d-flex child-flex" cols="6" md="3">
              <v-img
                :src="require(`../assets/${n}.jpg`)"
                aspect-ratio="1"
                class="grey lighten-2"
              >
                <template v-slot:placeholder>
                  <v-row
                    class="fill-height ma-0"
                    align="center"
                    justify="center"
                  >
                    <v-progress-circular
                      indeterminate
                      color="grey lighten-5"
                    ></v-progress-circular>
                  </v-row>
                </template>
              </v-img>
            </v-col>
          </v-row>
        </v-container>
    </v-app>
</template>
<script>
export default {
  name: 'Gallery',
  data() {
      return{
      }
  }
}
</script>
<style scoped>
.heading{
  color: #293e40;
  padding-bottom: 10px;
  text-align: center;
}
.section5 {
  margin-bottom: 50px;
}
.custom-btn-link{
  text-align: center;
  padding: 10px 0;
  font-size: 12px;
  text-decoration: none;
  color: #ffffff;
}
.custom-btn .btn{
  border-radius: 30px;
}
.v-btn:not(.v-btn--round).v-size--default{
  min-width: 15%;
}
@media only screen and (max-width: 600px) {
  .heading{
    font-size: 1.25rem;
  }
}
</style>