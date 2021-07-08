<template>
  <div>
    <v-container>
      <h2 class="heading">Qualifications</h2>
      <v-row>
        <v-col cols="12" lg="6">
          <div>
            <v-card outlined>
              <v-list-item three-line>
                <v-list-item-avatar tile size="100" color="teal">
                  <div class="avatar-text">
                    <h4>1999</h4>
                    <h5>1999</h5>
                    <h6>1999</h6>
                  </div>
                </v-list-item-avatar>
                <div class="vertical-border"></div>
                <v-list-item-content>
                  <v-list-item-subtitle>
                    Ph.D Food Technology
                  </v-list-item-subtitle>
                  <v-list-item-subtitle>
                    M.Sc. Food Technology
                  </v-list-item-subtitle>
                  <v-list-item-subtitle>
                    B.Sc. (Hons), Food Science & Technology
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-card>
          </div>
        </v-col>
        <v-col cols="12" lg="6">
          <div>
            <v-card outlined>
              <v-list-item three-line>
                <v-list-item-avatar tile size="100" color="teal">
                  <div class="avatar-text">
                    <h4>2009</h4>
                  </div>
                </v-list-item-avatar>
                <div class="vertical-border"></div>
                <v-list-item-content>
                  <v-list-item-subtitle>
                    Teilnahmebestaetigung (German Lang. A1 and A2)
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-card>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
};
</script>
<style scoped>
.avatar-text {
  display: block;
  line-height: 2em;
  color: rgb(189, 199, 255);
}
.vertical-border {
  position: relative;
  margin: 0 auto;
  width: 3px;
  height: 90px;
  border-left: 2px solid #91adaf;
  opacity: 0.9;
  margin-right: 10px;
}
.heading {
  color: #293e40;
  padding-bottom: 10px;
  text-align: center;
}
</style>