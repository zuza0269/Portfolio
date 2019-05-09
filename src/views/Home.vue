<template>
<v-app style="background: #f0f0f0">
  <v-container id="cont_home">
  <v-layout row>
      <v-flex xs6 id="navi">
         <v-navigation  class="subheading font-weight-light text-uppercase">
       <router-link id="home" class="black--text" to="/">Home</router-link>
      <router-link id="details" class="black--text" to="/details">Deta.ls</router-link> 
          <router-link id="design" class="black--text" to="/design">Des.gn</router-link> 
           <router-link id="contact" class="black--text" to="/contact">Contact</router-link> 
      <router-view></router-view>
          <hr tile flat id="navline">  
         
        </v-navigation>  
        </v-flex>
          <!-- title -->
         <v-flex xs6 order-lg2>
           <v-card tile flat style="background: #f0f0f0">
        <v-card tile flat style="background: #f0f0f0">
          <v-card-text>
  <h1 class="text-uppercase" id="devel-title">Front
      <br>
      -end
      <br>
      developer
      <br>
    </h1>
     <!-- expand btn -->
 <div class="text-xs-center">
    <v-layout justify-space-around>
      <v-btn id="expand"
      flat 
      tile
       style="background: rgba(139, 112, 245, 0.300)"
        @click="expand = !expand"
      >➝</v-btn>
    </v-layout>

    <v-expand-transition>
      <div v-show="expand">
       <hr id="ver-line">
             <h1 class="text-uppercase" id="port-title">
       Port
       <br>
       fol.o
             </h1>
          
       
      </div>
    </v-expand-transition>
  </div>
     
          </v-card-text>
        </v-card>
           </v-card>
      </v-flex>
    
      <v-flex xs6>
       <v-parallax id="img_me" :src="require('../assets/home/me.svg')">
   </v-parallax>
 
 

      </v-flex>
    </v-layout>
  </v-container>

  <!--first-component-->
   <aboutme>
 </aboutme>

<!--second-component-->
 <littled>
 </littled>

 <!--thrid component-->
<videod>
</videod>
</v-app>

</template>

<script>
import littled from  '../components/littled'
import aboutme from '../components/aboutme' 
import videod from '../components/videod'
  export default {
    name: 'home',
   components: {
      'aboutme':aboutme,
      'littled':littled,
      'videod':videod,
    },
    data: () => ({
      expand: false
    })
  }
</script>
<style lang="scss">
  h1 {
    letter-spacing:0.2em;
    font-size: 3.7vh;
  }
@mixin position ($pR, $T, $L, $tR) {
position: $pR;
top: $T;
left: $L;
text-align: $tR;
}
#devel-title {
  @include position (relative, 0, -130%, right);
}
#port-title {
  @include position (relative, 10%, -25%, left);
  }
#img_me {
width: 50vh;
position: relative;
left: -100%;
  }
  #ver-line {
    transform: rotate(90deg);
      border-top: solid #000 0.1vh;
      position: relative;
      left: -80%;
  }
  #expand {
    width: 35vh;
    height: 3vh;
    font-size: 2.3vh;
    position: relative;
    left: -100%;
  }
  #expand:hover {
    filter: blur(0.1vh);
   }

  /*navigation styling */

  #home {
    right: 2% ;
    top: 15%;
    letter-spacing:0.4em;
    transform: rotate(-90deg);
    font-size: 2.6vh;
     text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  }
  #home:hover {
    filter: blur(0.2vh);
  }
  #details {
    right: 3.8% ;
    top: 34%;
    letter-spacing:0.4em;
    font-size: 2.6vh;
    z-index: 1000;
     text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  }
    #details:hover {
    filter: blur(0.2vh);
  }
  #design {
    right: 3.5% ;
    top: 75%;
    letter-spacing:0.4em;
    font-size: 2.6vh;
    z-index: 1000;
     text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  }
    #design:hover {
    filter: blur(0.2vh);
  }
    #contact {
    right: 0.2%;
    top: 55%;
    letter-spacing:0.4em;
    transform: rotate(-90deg);
    font-size: 2.6vh;
     text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  }
  #contact:hover {
    filter: blur(0.2vh);
  }
  #navline {
  position: fixed;
  top: 0;
  border-left: 0.5vh solid rgba(139, 112, 245, 0.650);
  height: 100vh;
  right: 6.7%;
  }


</style>