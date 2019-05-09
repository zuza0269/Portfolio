<template>
   <v-app style="background: #f0f0f0">
        <v-container fluid>
 <v-layout row wrap>
      <v-flex xs12 sm6 md3 order-md4 order-sm2>
     <v-img data-aos="zoom-in" data-aos-duration="1000" id="astro2" :src="require('../assets/design/astro2.png')"/>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md3 order-sm1>
    <v-img data-aos="zoom-in" data-aos-duration="1500" id="astro4" :src="require('../assets/design/astro4.png')"/>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md2 order-sm4>
        <v-img data-aos="zoom-in" data-aos-duration="2000" id="astro3" :src="require('../assets/design/astro3.png')"/>
      </v-flex>
      <v-flex xs12 sm6 md3 order-md1 order-sm3>
      <v-img data-aos="zoom-in" data-aos-duration="1000" id="astro1" :src="require('../assets/design/astro1.png')"/>
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