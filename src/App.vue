<template>
<div>
 <v-tabs
    centered
    color="black"
    dark
    icons-and-text
    class="white--text"
  >
    <v-tabs-slider color="white"></v-tabs-slider>

    <v-tab href="#tab-1">
      Home
      <v-icon>home</v-icon>
    </v-tab>

    <v-tab href="#tab-2">
      Apps
      <v-icon>apps</v-icon>
    </v-tab>
  </v-tabs>

  <router-view></router-view>

<v-footer
    dark
    height="auto"
  >
    <v-card
      flat
      tile
      class="flex black white--text text-xs-center"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-3 white--text"
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
      </v-card-text>
      <v-divider></v-divider>

      <v-card-text class="white--text">
        &copy;2018 — <strong>Kauyumaribb Apps</strong>
      </v-card-text>

    </v-card>
  </v-footer>
</div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    icons: ['fab fa-facebook', 'fab fa-twitter', 'fab fa-google-plus', 'fab fa-linkedin', 'fab fa-instagram']
  })
}
</script>

<style>
</style>
