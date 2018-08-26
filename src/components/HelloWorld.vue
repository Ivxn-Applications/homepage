<template>
  <v-content>
    <section>
      <v-parallax :src="require('@/assets/chaquira.jpg')" height="250">
      </v-parallax>
    </section>

    <section>
        <v-jumbotron :gradient="gradient" dark height="250" :src="require('@/assets/chaquira.jpg')">
          <v-container fill-height>
            <v-layout align-center>
              <v-avatar
                :tile="tile"
                :size="200"
                class="text-xs-left">
                <img src="./../assets/profileimage.jpg" alt="avatar">
              </v-avatar>
            </v-layout>
          </v-container>
        </v-jumbotron>
    </section>

    <section>
       <v-parallax :src="require('@/assets/chaquira.jpg')" height="250">
      </v-parallax>
    </section>

       <section>
        <v-jumbotron :gradient="gradient" dark height="250" class="elevation-20" :src="require('@/assets/chaquira.jpg')">
          <v-container fill-height>
            <v-layout align-center>
              <v-avatar
                :tile="tile"
                :size="200"
                class="text-xs-left">
                <img src="./../assets/profileimage.jpg" alt="avatar">
              </v-avatar>
            </v-layout>
          </v-container>
        </v-jumbotron>
    </section>

  </v-content>
</template>

<script>
export default {
  data: () => ({
    gradient: 'to top, #FFFFFF, transparent'
  })
}
</script>
