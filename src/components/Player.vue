<template>
  <v-container class="root-container">
    <div class="player-outter-container">
      <div class="player-inner-container">
        <span class="display-1 track-description">
          track title &#8226;
          <span class="track-artist">track artist</span>
        </span>
        <v-icon large>
          mdi-play
        </v-icon>
      </div>
    </div>
    <div class="nav-container">
      <v-row align="center" justify="space-around" no-gutters class="nav-row">
        <v-btn value="recent">
          <span class="subtitle-1">Home</span>
          <v-icon large>mdi-home</v-icon>
        </v-btn>

        <v-btn value="favorites">
          <span class="subtitle-1">Search</span>
          <v-icon large>mdi-magnify</v-icon>
        </v-btn>

        <v-btn value="nearby">
          <span class="subtitle-1">Playlists</span>
          <v-icon large>mdi-playlist-music</v-icon>
        </v-btn>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "Player"
};
</script>

<style scoped>
.root-container {
  display: flex;
  flex-direction: column;
  padding: 0;
  background-color: #282828;
}

.player-outter-container {
  border-bottom: 0.1rem solid #1f1f1f;
}

.player-inner-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.8rem 2rem;
}

.nav-container {
  flex-grow: 1;
}

.nav-row {
  height: 100%;
  padding: 0 1.2rem;
}

.rack-description {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
  max-width: 90%;
}

.track-artist {
  color: #858585;
}
</style>
