<template>
<v-app style="background: #f0f0f0">
  <v-container fluid>
    <!--first part-->
    <v-layout row justify-space-around="">
      <v-flex xs6 order-lg2>
        <v-parallax id="img_me2" :src="require('../assets/home/aboutme/me2.svg')">

      </v-parallax>
      </v-flex>

      <!--expand title about me -->
      <v-flex xs6>

       <v-card tile flat style="background: #f0f0f0">
          <v-card-title>
            <div class="text-xs-center">
   
      <v-btn id="Z"
        flat tile
       style="background: #f0f0f0"
        @click="expand = !expand"
      > <h1 id="first-let">> Z</h1>
    
      </v-btn>
    

    <v-expand-transition>
      <div v-show="expand">
  
       <hr id="ver-line">
             <h1 class="text-uppercase" id="about-title">
       About
       <br>
       me
             </h1>
            
      </div>
    </v-expand-transition>
  </div>
           <v-card-text v-show="expand" class="font-weight-light" id="text-aboutme">
            {{text1.aboutme}}
            <br>
            {{text2.aboutme}}

          </v-card-text>
            </v-card-title>
        </v-card>
       
      </v-flex>
    </v-layout>
<!-- second part -->
 <v-layout row>
      <v-flex xs6 order-lg>
        <v-card tile flat style="background: #f0f0f0">
         <v-parallax id="img_me3" :src="require('../assets/home/aboutme/me3.svg')">
          </v-parallax>
           </v-card>
      </v-flex>
      <v-flex xs6>
        
<v-card tile flat style="background: #f0f0f0">
         <v-card-text >
          <p  data-aos="fade-up" data-aos-duration="2500" class="text-uppercase font-weight-light" id="quote-text">transforming your
            <br>
            into
          </p>
          <p  data-aos="fade-up" data-aos-duration="2000" class="text-uppercase font-weight-black" id="quote-ideas">.deas</p>
           <p  data-aos="fade-up" data-aos-duration="1500" class="text-uppercase font-weight-black" id="quote-reality">real.ty</p>
           </v-card-text>
        </v-card>

       
      </v-flex>
    </v-layout>

  </v-container>
</v-app>
</template>

<script>
    export default {
      data: () => ({
      expand: false,
       text1: {aboutme:'My name is Zuzana Korinkova and right now I am a Multimedia Design student.'},
       text2: {aboutme:'I am mostly focusing on Web Design and Development.'}
     
    }),
    }
</script>

<style lang="scss" scoped>
 h1 {
    letter-spacing:0.2em;
    font-size: 3.7vh;
  }
  //first part
#img_me2 {
    width: 45vh;
    position: relative;
    left: 0;
}
#Z {
 position: relative;
 left: -20%;
 border-bottom: solid 0.1vh #000;
}
#first-let::first-letter {
  color: rgba(139, 112, 245, 0.650);
}
#Z:hover {
  filter: blur(0.1vh);
}
#ver-line {
  border: solid #000 0.05vh;
  position: relative;
  left: 7%;
}
#about-title {
  text-align: left;
  position: relative;
  left: 60%;
}
#text-aboutme {
 letter-spacing:0.1em;
 font-size: 3vh;
 line-height: 5vh;
 text-align: start;

}

//second part
#img_me3 {
   width: 45vh;
   position: relative;
}
#quote-text {
  letter-spacing: 0.1em;
  font-size: 3vh;
  position: absolute;
  top: 95%;
  text-align: right;
  z-index: 1000;
  left: -20%;
}
#quote-ideas {
  letter-spacing: 0.1em;
  font-size: 7vh;
  position: absolute;
  left: 12.5%;
  color:rgba(139, 112, 245, 0.300)
}
#quote-reality {
  letter-spacing: 0.1em;
  font-size: 7vh;
  position: absolute;
  left: 21%;
  top: 143%;
  color:rgba(139, 112, 245, 0.600)
}
</style>