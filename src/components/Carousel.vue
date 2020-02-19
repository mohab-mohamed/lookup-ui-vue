<template>
<div class="carouselContainer">
  <carousel-3d :controlsVisible='true' :perspective='50' :autoplay='true' :loop='true'>
      <slide :index="0">
        <img src="placeholder.png">
      </slide>
      <slide :index="1">
      </slide>
      <slide :index="3">
      </slide>
      <slide :index="4">
      </slide>
      <slide :index="5">
      </slide>
      <slide :index="6">
      </slide>
      <slide :index="7">
      </slide>
      <slide :index="8">
      </slide>
      <slide :index="9">
      </slide>
      <slide :index="10">
      </slide>
      <slide :index="11">
      </slide>
      <slide :index="12">
      </slide>
  </carousel-3d>
</div>
</template>

<script lang="ts">
import {
  Component,
  Prop,
  Vue
} from 'vue-property-decorator';
import {
  Carousel3d,
  Slide
} from 'vue-carousel-3d';

export default {
  components: {
    Carousel3d,
    Slide
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
    margin: 40px 0 0;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}
.carousel-3d-slide {
      border-radius: 60%;
      // width: 1vw;
      // height:10vw;
      background-color: rgba(0, 0, 0, 0.5) ;
    }
.pictureHolder {

}
.carouselContainer {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 100%;
  width: 100%;
}

</style>
