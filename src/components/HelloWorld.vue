<template>
 <section>
<v-parallax
    dark
    src="http://4.bp.blogspot.com/-Yguoj_alf-o/U_F44ddrlBI/AAAAAAAAANQ/Jt2s_UeR6-E/s1600/milky-way-derek-rowley-derekscope.jpg"
    height='900'
  >
    <v-layout
      align-center
      column
      justify-center
    >
      <v-avatar
            :size=254
            color="transparent"
          >
            <img class="elevation-24" :src="require('@/assets/kauyumari.png')" alt="avatar">
      </v-avatar>
    </v-layout>

    <v-jumbotron :gradient="gradient" dark height="300" class="elevation-20">
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
  </v-parallax>
</section>

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
<style>

</style>
