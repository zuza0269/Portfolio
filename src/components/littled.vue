<template>
<v-app style="background: #f0f0f0">
   <v-container>
      <v-layout row wrap>
      <v-flex xs12 sm6 md3 order-md4 order-sm2>
       <img data-aos="zoom-in" data-aos-duration="1000" id="img_work2" :src="require('../assets/home/d/work2.png')"/> 
       <hr tile flat id="hor-line1">
      </v-flex>
      <v-flex xs12 sm6 md3 order-md3 order-sm1>
         <img data-aos="zoom-in" data-aos-duration="1200" id="img_work3" :src="require('../assets/home/d/work3.png')"/>
             <hr id="ver-line1">
      </v-flex>
      <v-flex xs12 sm6 md3 order-md2 order-sm4>
       <img data-aos="zoom-in" data-aos-duration="900" id="img_work1" :src="require('../assets/home/d/work1.png')"/>
        <hr id="hor-line2">
      </v-flex>
      <v-flex xs12 sm6 md3 order-md1 order-sm3>
         <v-card  tile flat style="background: #f0f0f0" id="quote-d">
          <v-card-title  data-aos="fade-up" data-aos-duration="2500"  id="title-d" class="text-uppercase font-weight-black">Des.gn</v-card-title>
          <v-card-text  id="text-d" class="text-uppercase font-weight-light">is the silent ambassador of your brand</v-card-text>
  
              <hr id="ver-line2">
        </v-card>
      </v-flex>
      
    </v-layout>
    
   </v-container>
</v-app>
    
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

@mixin pos-all ($pR, $L, $R, $T) {
  position: $pR;
  left: $L;
  right: $R;
  top: $T;
}
#img_work1 {
    width: 65vh;
    @include pos-all (relative, -100%, 0, 0);
}
#img_work3 {
  width: 35vh;
     @include pos-all (relative, 10%, 0, 0);
}
#img_work2 {
  width: 65vh;
  @include pos-all (relative, -120%, 0, 120%);
}
#quote-d {
  @include pos-all (relative, 0, 0, 120%);
}
#title-d {
  font-size: 10vh;
  letter-spacing: 0.2em;
  color:rgba(139, 112, 245, 0.600);
}
#text-d {
 letter-spacing: 0.2em;
 font-size: 2.5vh;
  @include pos-all (absolute, 57%, 0, 60%);
}
#hor-line1 {
   background-color: rgba(139, 112, 245, 0.500);
height: 0.4vh;
border-style: none;
   transform: rotate(90deg);
@include pos-all (absolute, 28%, 0, 32%);
width: 50vh;
}
#ver-line1 {
     background-color: rgba(139, 112, 245, 0.500);
height: 0.4vh;
border-style: none;
@include pos-all (absolute, 35%, 0, 51%);
width: 50vh;
}
#hor-line2 {
      background-color: rgba(0, 0, 0, 0.500);
height: 0.4vh;
border-style: none;
   transform: rotate(90deg);
@include pos-all (absolute, 33.3%, 0, 75%);
width: 30vh;
}
#ver-line2 {
        background-color: rgba(0, 0, 0, 0.500);
height: 0.4vh;
border-style: none;
@include pos-all (absolute, 63%, 0, -29.3%);
width: 30vh;
}
/*responsiveness*/
@media only screen and (max-width: 960px) {
#img_work1 {
    @include pos-all (none,0, 0, 0);
}
#img_work3 {
  @include pos-all (none,0, 0, 0);
}
#img_work2 {
@include pos-all (none,0, 0, 0);
}
#quote-d {
@include pos-all (none,0, 0, 0);
}
#text-d {
@include pos-all (relative,0, 0, 0);
}
#name-d {
@include pos-all (relative,0, 0, 0);
}

} 
@media only screen and (max-width: 1270px) {
#hor-line1 {
display: none;
}
#ver-line1 {
display: none;
}
#hor-line2 {
display: none;
}
#ver-line2 {
display: none;
}
}
#container {
  position: relative;
  top: 50%;
}
@media screen and (min-width: 1281px) {
#hor-line1 {
display: none;
}
#ver-line1 {
display: none;
}
#hor-line2 {
display: none;
}
#ver-line2 {
display: none;
}
 }
 
</style>