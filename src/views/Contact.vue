<template>
   <v-app style="background: #f0f0f0">
 <router-link id="home-details" class="text-uppercase font-weight-light black--text" to="/">← Home</router-link>
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
        <v-card flat tile style="background-color: #f0f0f0">
          <v-card-text id="cont" class="text-uppercase font-weight-black">Contact</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
      </v-container>
      <v-container fluid>
<v-layout justify-space-around>
      <v-flex
        xs9
      >
         <v-img id="img_cont" :src="require('../assets/contact/contact.svg')"/>
         <p id="ln-text" class="text-uppercase font-weight-light">l.nked .in</p>
         <a href="https://www.linkedin.com/in/zuzana-korinkova/" target="_blank"> <v-img id="img_ln" :src="require('../assets/contact/ln.svg')"/> </a> 
         <p id="em-text" class="text-uppercase font-weight-light">ema.l</p>
         <a href="mailto:korinkova.zuzana3@gmail.com"> <v-img id="img_em" :src="require('../assets/contact/em.svg')"/> </a> 
         <p id="lc-text" class="text-uppercase font-weight-light">locat.on</p>
<div >

      <v-img  @click="expand = !expand" id="img_lc" :src="require('../assets/contact/lc.svg')"/> 


    <v-expand-transition>
      <div v-show="expand">
             <p class="font-weight-light" id="exp-text">
     Jernbanegade 14
     <br>
     Esbjerg, DK
             </p>
          
       
      </div>
    </v-expand-transition>
  </div>
     




        
      </v-flex>
  </v-layout>
  </v-container>


 
   </v-app>
</template>

<script>
    export default {
          data: () => ({
      expand: false
    })
    }
</script>

<style lang="scss" scoped>
#home-details {
   text-decoration: none;
    letter-spacing: 0.4em;
    position: fixed;
  z-index: 1000;
}
#home-details:hover {
  filter: blur(0.2vh);
}
#cont {
    letter-spacing: 0.5em;
    font-size: 9vh;
    color: rgba(139, 112, 245, 0.200);
}
#img_cont {
    width: 130vh;
    background-position: center;
}
#ln-text {
    position: relative;
    font-size: 3vh;
    letter-spacing: 0.2em;
    top: -44%;
    left: 9%;
}
#em-text {
     position: relative;
    font-size: 3vh;
    letter-spacing: 0.2em;
    top: -50%;
    left: 43%;
}
#lc-text {
     position: relative;
    font-size: 3vh;
    letter-spacing: 0.2em;
    top: -65%;
    left: 71%;
 }
 #img_ln {
     width: 13.5vh;
    position: absolute;
  top: 47%;
  left: 22%;
 }
 #img_ln:hover {
transform: scale(1.3);
 }
  #img_em {
     width: 8vh;
    position: absolute;
  top: 50%;
  left: 47%;
 }
  #img_em:hover {
transform: scale(1.3);
 }
 #img_lc {
     width: 3vh;
    position: absolute;
  top: 44%;
  left: 70.5%;
 }
 #img_lc:hover {
transform: scale(1.3);
 }
 #exp-text {
     position: absolute;
     letter-spacing: 0.2em;
     top: 50%;
  left: 63.5%;

 }

</style>