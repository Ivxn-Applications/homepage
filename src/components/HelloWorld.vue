<template>
  <v-content>
    <section>
      <v-parallax :src="require('@/assets/chaquira.jpg')" height="300">
      </v-parallax>
    </section>

    <section>
        <v-jumbotron color="colorparallax" dark height="300" :src="require('@/assets/chaquira.jpg')">
          <v-container fill-height>
            <v-layout align-center>
              <v-avatar
                :tile="tile"
                class="text-xs-center">
                <img src="./../assets/profileimage.jpg" alt="avatar">
              </v-avatar>
            </v-layout>
          </v-container>
        </v-jumbotron>
    </section>

    <section>
       <v-parallax :src="require('@/assets/chaquira.jpg')" height="300">
      </v-parallax>
    </section>

       <section>
        <v-jumbotron :gradient="gradient" dark height="300" class="elevation-20" :src="require('@/assets/chaquira.jpg')">
          <v-contaner fill-height>
            <div class="flex white--text display-1 text-xs-center">Delivering the best solution</div>
          </v-contaner>
          <v-container fill-height>
             <v-layout
                align-center
                justify-space-around
                wrap
              >
              <v-avatar v-for="icon in icons"
              :key="icon"
              >
                <img :src="require('@/assets/'+icon+'.png')">
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
    colorparallax: 'transparent',
    gradient: 'to top, #000000, transparent',
    icons: ['angular', 'vue', 'nodejs', 'java', 'python', 'qt', 'kb8', 'docker', 'rasp']
  })
}
</script>
