<template>
  <v-app>
    <v-navigation-drawer app v-show="$vuetify.breakpoint.smAndUp">
    </v-navigation-drawer>
    <v-content>
      <v-container fluid>
        <router-view></router-view>
      </v-container>
    </v-content>
    <!-- <v-footer app padless class="footer">
      <PlayerTrackDetails />
    </v-footer> -->
    <v-bottom-navigation v-show="$vuetify.breakpoint.xsOnly" height="110">
      <Player />
    </v-bottom-navigation>
  </v-app>
</template>

<script>
import Player from "./components/Player";

export default {
  name: "App",
  components: {
    Player
  },
  data: () => ({
    //
  })
};
</script>

<style>
*::selection {
  opacity: 1;
  background: rgba(255, 255, 255, 0.99) !important;
  color: #0078d7 !important;
}
/* .v-application p {
  margin-bottom: 0 !important;
} */
/* .footer {
  height: 9rem;
} */
</style>
