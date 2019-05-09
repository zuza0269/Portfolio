<template>
  <v-app style="background: #f0f0f0;">
     <v-container fluid id="container">
    <v-layout row>
      <v-flex xs6 order-lg2>
       <v-img id="img_websam" :src="require('../assets/home/websam.svg')"/>
      </v-flex>
      <v-flex xs6>
  <div class="text-xs-center" id="card1">
    <v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on }">
        <v-btn
          style="background-color: #f0f0f0"
          class="text-uppercase font-weight-light" id="somelink1"
          flat tile
          v-on="on"
        >
          website with keyframe animations and sass
        </v-btn>
      </template>

      <v-card>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/SMViKLXnSgA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
       
        

      </v-card>
    </v-dialog>
  </div>
   <div class="text-xs-center" id="card2">
    <v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on }">
        <v-btn
          style="background-color: #f0f0f0"
          class="text-uppercase font-weight-light" id="somelink2"
          flat tile
          v-on="on"
        >
          website with horizontal scrolling
        </v-btn>
      </template>

      <v-card>
     <iframe width="560" height="315" src="https://www.youtube.com/embed/S5fVoK-2Iu0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
       
      </v-card>
    </v-dialog>
  </div>
    </v-flex>
    <v-flex>
      
    </v-flex>
  </v-layout>
</v-container>
  </v-app>
</template>


<script>
    export default {
        data() {
           return {
        dialog: false
      }
        }
    }
</script>

<style lang="scss" scoped>
#container {
  position: relative;
  top: 5%;
}
#somelink1 {
  position: relative !important;
  letter-spacing: 0.2em !important;
  text-decoration: none;
  color: #000;
}
#somelink1:hover {
  filter:blur(0.2vh);
}
#somelink2 {
  position: relative !important;
  letter-spacing: 0.2em !important;
  justify-content: right;
  text-decoration: none;
  color: #000;
}
#somelink2:hover {
  filter:blur(0.2vh);
}

#img_websam {
  width: 60vh;
}
#card1 {
  position: relative;
  top: 15%;
}
#card2 {
  position: relative;
  top: 15%;
}
</style>