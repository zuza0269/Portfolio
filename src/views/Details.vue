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
          <v-card-text id="det" class="text-uppercase font-weight-black">Deta.ls</v-card-text>
          <div class="text-xs-center">
  
      <v-btn
        id="exp-btn" flat tile
        @click="expand = !expand"
      > </v-btn>
    

    <v-expand-transition>
      <div v-show="expand">
        <p id="p1" class="text-uppercase font-weight-light">Dec 97</p>
      </div>
    </v-expand-transition>
  </div>
        </v-card>
      </v-flex>
    </v-layout>
      <v-layout row
      id="edu">
       <v-flex
        grow
        pa-1 
      >
       </v-flex>

       <!--Education-->
      <v-flex
        grow
        pa-1 
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-title id="edu-title1" class="text-uppercase font-weight-regular">Educat.on</v-card-title>
        </v-card>
        
      </v-flex>
       <v-flex
        grow
        pa-1 
      >
       </v-flex>
    </v-layout>
    
  </v-container>
  <v-container fluid>
  <v-layout row>
     
      <v-flex
        shrink
        pa-1
      >
       
         <v-parallax id="img_me4" :src="require('../assets/details/me4.svg')">

      </v-parallax>
    
      </v-flex>
       <v-flex
        grow
        pa-1
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="1000" id="text" class="font-weight-light"> Aug 18 - now : AP Degree > Multimedia Design and Communication </v-card-text>
            <v-card-text data-aos="fade-up" data-aos-duration="2000" id="text-under" class="font-weight-light"> Business Academy South West, DK </v-card-text>
        </v-card>
          <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="1000" id="text" class="font-weight-light"> Sept 13 - May 17 : Graduate > International Business  </v-card-text>
            <v-card-text data-aos="fade-up" data-aos-duration="2000" id="text-under" class="font-weight-light"> Thomas Bata Business Academy, CZ</v-card-text>
        </v-card>
      </v-flex>
      
     
    </v-layout>

 <!--Experience-->
     <v-layout row>
    
      <v-flex
        grow
        pa-1 
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-title id="edu-title2" class="text-uppercase font-weight-regular">Exper.ence</v-card-title>
        </v-card>
        
      </v-flex>
       <v-flex
        grow
        pa-1 
      >
       </v-flex>
    </v-layout>
    
  </v-container>

  <v-container fluid>
  <v-layout row>
       <v-flex
        grow
        pa-1
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="1000" id="text" class="font-weight-light"> April 16  : Internship > Administrative assistant in Purple Telecom </v-card-text>
            <v-card-text data-aos="fade-up" data-aos-duration="2000" id="text-under" class="font-weight-light"> ERASMUS+, Plymouth, UK </v-card-text>
        </v-card>
          <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="1000" id="text" class="font-weight-light"> Mar 18th - 29th 19  : Study trip > Prototyping, Experience Economy </v-card-text>
            <v-card-text data-aos="fade-up" data-aos-duration="2000" id="text-under" class="font-weight-light"> Saxion University, Enschede, NL </v-card-text>
        </v-card>
      </v-flex>
     
      <v-flex
        shrink
        pa-1
      >
       
         <v-parallax id="img_me4" :src="require('../assets/details/me5.svg')">

      </v-parallax>
    
      </v-flex>
     
    </v-layout>
   

<!--Skills-->
  <v-layout row>
    
      <v-flex
        grow
        pa-1 
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-title id="edu-title3" class="text-uppercase font-weight-regular">Sk.lls</v-card-title>
        </v-card>
        
      </v-flex>
       <v-flex
        grow
        pa-1 
      >
       </v-flex>
    </v-layout>
     </v-container>
   <v-container fluid>
  <v-layout row wrap>
      <v-flex xs12 sm6 md3 order-md4 order-sm2>
        <v-card tile flat style="background: #f0f0f0">
              <v-card-title data-aos="fade-up" data-aos-duration="900" id="title"  class="font-weight-light text-uppercase"> Vue</v-card-title>
          <v-card-text data-aos="fade-up" data-aos-duration="2000"  class="font-weight-light" >
            <p>VUE CLI</p>
             <p>VUETIFY</p>
              <p>VUE.JS</p>
            </v-card-text>
        
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md3 order-sm1>
         <v-card tile flat style="background: #f0f0f0">
           <v-card-title data-aos="fade-up" data-aos-duration="900"  id="title"  class="font-weight-light text-uppercase"> Extra</v-card-title>
          <v-card-text data-aos="fade-up" data-aos-duration="2000"   class="font-weight-light" >
            <p>SASS</p>
             <p>XAMPP</p>
              <p>WORDPRESS</p>
            </v-card-text>
        
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md2 order-sm4>
          <v-card tile flat style="background: #f0f0f0">
            <v-card-title data-aos="fade-up" data-aos-duration="900"  id="title"  class="font-weight-light text-uppercase"> Adobe</v-card-title>
          <v-card-text data-aos="fade-up" data-aos-duration="2000"  class="font-weight-light" >
            <p>ILLUSTRATOR</p>
             <p>XD</p>
              <p>PHOTOSHOP</p>
            </v-card-text>
        
        </v-card>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md1 order-sm3>
         <v-card tile flat style="background: #f0f0f0">
           <v-card-title data-aos="fade-up" data-aos-duration="900"  id="title"  class="font-weight-light text-uppercase"> Basics</v-card-title>
          <v-card-text data-aos="fade-up" data-aos-duration="2000" class="font-weight-light" >
            <p>HTML</p>
             <p>CSS</p>
              <p>JAVASCRIPT</p>
            </v-card-text>
         </v-card>
      </v-flex>
    </v-layout>
 </v-container>
    <!--Personality-->
    <v-container fluid>
     <v-layout row>
    
      <v-flex
        grow
        pa-1 
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-title id="edu-title4" class="text-uppercase font-weight-regular">Personal.ty</v-card-title>
        </v-card>
        
      </v-flex>
       <v-flex
        grow
        pa-1 
      >
       </v-flex>
    </v-layout>
    
    </v-container>
     <v-container fluid>
  <v-layout row>
     
      <v-flex
        shrink
        pa-1
      >
       
         <v-parallax id="img_me4" :src="require('../assets/details/me6.svg')">

      </v-parallax>
    
      </v-flex>
       <v-flex
        grow
        pa-1
      >
        <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="900" id="person" class="font-weight-light"> I am hardworking and like to challenge myself  </v-card-text>
        </v-card>
          <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="1000" id="person-op" class="font-weight-light"> I have creative mind </v-card-text>
        
        </v-card>
         <v-card tile flat
          style="background: #f0f0f0"
        >
          <v-card-text data-aos="fade-up" data-aos-duration="2000" id="person-col" class="font-weight-light"> I am good listener and observer </v-card-text>
        
        </v-card>
      </v-flex>
        <v-flex
        shrink
        pa-1
      >
       
         <v-img id="img_infj" :src="require('../assets/details/infj.svg')"/>

     
    
      </v-flex>
     
    </v-layout>
     </v-container>
</v-app>
</template>

<script>
    export default {
      data: ()  => ({
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
#det {
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
    left: -14.6%;
}
#exp-btn:hover {
    filter: blur(0.2vh);
}
#p1 {
    transform: rotate(90deg);
    position: relative;
    left: -14.6%;
    color: rgb(139, 112, 245);
}
#edu {
  position: relative;
  top: 25%;
}
#edu-title1 {
  letter-spacing: 0.2em;
  font-size: 7vh;
  color: rgba(0, 0, 0, 0.50);
  position: relative;
  left: 30%;
}
#edu-title2 {
  letter-spacing: 0.2em;
  font-size: 7vh;
  color: rgba(0, 0, 0, 0.50);
  position: relative;
  left: 30%;
}
#edu-title3 {
  letter-spacing: 0.2em;
  font-size: 7vh;
  color: rgba(0, 0, 0, 0.50);
  position: relative;
  left: 60%;
}
#edu-title4 {
  letter-spacing: 0.2em;
  font-size: 7vh;
  color: rgba(0, 0, 0, 0.50);
  position: relative;
  left: 40%;
}

#img_me4 {
  width: 40vh;
}
#text {
  letter-spacing: 0.4em;
  font-size: 2.5vh;
}
#text-under {
  letter-spacing: 0.4em;
  color:  rgba(139, 112, 245, 0.400);
  font-size: 4vh;
  position: absolute;
  top: 16%;
}
p {
  letter-spacing: 0.2em;
  text-align: center;
}
#title { 
  letter-spacing: 0.2em;
   color:  rgba(139, 112, 245, 0.400);
   font-size: 5vh;

}
#img_infj {
  width: 50vh;
}
#person {
   letter-spacing: 0.2em;
   font-size: 2vh;
}
#person-op {
   letter-spacing: 0.2em;
   font-size: 2vh;
   color: rgba(0, 0, 0, 0.500);
   text-align: center;
}
#person-col {
   letter-spacing: 0.2em;
   font-size: 2vh;
   color:rgba(139, 112, 245, 0.700);
   text-align: right;
}
</style>