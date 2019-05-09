<template>
 <v-app style="background: #f0f0f0;">
 <router-link id="home-des" class="text-uppercase font-weight-light black--text" to="/">← Home</router-link>
  <v-container>
    <v-layout row>
      <v-flex
        grow
        pa-1
      >
       
      </v-flex>
      <v-flex
        grow
      >
        <v-card flat tile style="background-color: #f0f0f0;">
          <v-card-text id="des" class="text-uppercase font-weight-black">Des.gn</v-card-text>
           <div class="text-xs-center">
  
      <v-btn
        id="exp-btn" flat tile
        @click="expand = !expand"
      > </v-btn>
    

    <v-expand-transition>
      <div v-show="expand">
        <p id="p" class="text-uppercase font-weight-light">adobe</p>
      </div>
    </v-expand-transition>
  </div>
        </v-card>
      </v-flex>
    </v-layout>
   
      </v-container>
      <v-container>
        <v-layout row>
  <v-flex
        grow
        pa-1 
      >
        <v-card tile flat id="astro-title"
          style="background: #f0f0f0"
        >
          <v-card-title  class="text-uppercase font-weight-regular">
            <p  data-aos="fade-right" data-aos-duration="1000">  Astronomy |</p>
            <p data-aos="fade-right" data-aos-duration="2000">| Project | </p>
            <p data-aos="fade-right" data-aos-duration="3000">| Space  </p>
         
            </v-card-title>
        </v-card>
        
      </v-flex>
       <v-flex
        grow
        pa-1 
      >
       </v-flex>
</v-layout>
</v-container>

     <imaged>

     </imaged>
 </v-app>
</template>

<script>
import imaged from '../components/imaged'
  export default {
    components: {
      'imaged':imaged,
    },
      data: ()  => ({
      expand: false
     })
  }
</script>

<style lang="scss" scoped>
#home-des {
   text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  z-index: 1000;
}
#home-des:hover {
  filter: blur(0.2vh);
}
#des {
    letter-spacing: 0.5em;
    font-size: 9vh;
    color: rgba(139, 112, 245, 0.200);
}
#exp-btn {
border: solid #000 0.1vh;
    transform: rotate(90deg);
    width: 26vh;
    height: 3vh;
    position: relative;
    left: -22%;
     }
    #p {
    transform: rotate(90deg);
    position: relative;
    left: -22%;
    color: rgb(139, 112, 245);
}
#astro-title {
  letter-spacing: 0.2em;
  font-size: 4vh;
  color: rgba(0, 0, 0, 0.50);
  position: relative;
  top: 20%;
}
@mixin astro_pos ($pR, $L, $T) {
  position: $pR;
  left: $L;
  top: $T;
}
#astro1 {
  @include astro_pos (relative, 0, 0)
}
#astro2 {
  @include astro_pos (relative, 0, 60%)
}
#astro3 {
  @include astro_pos (relative, -30%, 60%)
}
#astro4 {
  @include astro_pos (relative, -15%, 0)
}
@media only screen and (max-width: 1270px) {
#astro1 {
  @include astro_pos (relative, 0, 0)
}
#astro2 {
  @include astro_pos (relative, 0, 0)
}
#astro3 {
 @include astro_pos (relative, 0, 0)
}
#astro4 {
  @include astro_pos (relative, 0, 0)
}
 }
</style>