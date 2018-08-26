<template>
<div>
 <v-tabs
    centered
    color="cyan"
    dark
    icons-and-text
  >
    <v-tabs-slider color="yellow"></v-tabs-slider>

    <v-tab href="#tab-1">
      Home
      <v-icon>home</v-icon>
    </v-tab>

    <v-tab href="#tab-2">
      Apps
      <v-icon>apps</v-icon>
    </v-tab>

    <v-tab href="#tab-3">
      Photography
      <v-icon>photo_library</v-icon>
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
      class="cyan lighten-1 white--text text-xs-center"
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

      <v-card-text class="white--text pt-0">
        Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
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
