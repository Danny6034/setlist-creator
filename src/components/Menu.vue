<template>
<div class="menu">
    <v-btn class="custom-button" @click="refreshUserInfo"> Get User Info </v-btn>
    <v-btn class="custom-button"  @click="refreshPlaylists"> Get Playlists </v-btn>
</div>
</template>

<script>
import * as auth from "../api/auth.js";

export default {
  methods: {
    refreshUserInfo() {
      auth.refreshUserInfo();
    },
    refreshPlaylists() {
        auth.refreshPlaylists();
    }
  }
}
</script>

<style scoped>
.menu {
    text-align: center;
}

.custom-button {
  color :"#CDCACC";
}
</style>