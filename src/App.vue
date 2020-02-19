<template>
<div class="fullContainer">
  <div class="topContainer">
  </div>
  <div class="logoContainer">
    <Carousel />
  </div>
  <div class="bottomContainer">
    <div class="wrap">
     <div class="search">
        <input type="text" class="searchTerm" placeholder="Who are you looking for?">
        <button type="submit" class="searchButton">
          <i class="fa fa-search"></i>
       </button>
     </div>
  </div>

  </div>
</div>
</template>

<script lang="ts">
import {
  Component,
  Vue
} from 'vue-property-decorator';
import Carousel from './components/Carousel.vue';

@Component({
  components: {
    Carousel,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
@bg-color: #913D88;
@txt-color: #FFFFFF;

#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
.fullContainer {
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100%;
    background: linear-gradient(306deg, #005daa, #17468f, #002c70, #002256);
    background-size: 800% 800%;

    -webkit-animation: AnimationName 24s ease infinite;
    -moz-animation: AnimationName 24s ease infinite;
    animation: AnimationName 24s ease infinite;

    justify-content: space-evenly;
    align-items: center;

}
.logoContainer {
    background-image: url("rbc-logo.png");
    width: 100%;
    height: 40vw;
    background-repeat: no-repeat;
    background-size: 40vw 40vw;
    // margin-bottom: 1vh;
    // background-size: cover;
    background-position: center;
    opacity: 0.3;
}
.topContainer {
    height: 1vw;
    width: 100%;
}
.bottomContainer {
    height: 1vw;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

@-webkit-keyframes AnimationName {
    0% {
        background-position: 45% 0;
    }
    50% {
        background-position: 56% 100%;
    }
    100% {
        background-position: 45% 0;
    }
}
@-moz-keyframes AnimationName {
    0% {
        background-position: 45% 0;
    }
    50% {
        background-position: 56% 100%;
    }
    100% {
        background-position: 45% 0;
    }
}
@keyframes AnimationName {
    0% {
        background-position: 45% 0;
    }
    50% {
        background-position: 56% 100%;
    }
    100% {
        background-position: 45% 0;
    }
}
@import url(https://fonts.googleapis.com/css?family=Open+Sans);
.search {
  width: 100%;
  display: flex;
  flex-direction:row;
  justify-content: center;
  align-items: center;
}

.searchTerm {
  width: 100%;
  border: 1px solid white;
  border-right: none;
  padding: 5px;
  height: 20px;
  border-radius: 5px 0 0 5px;
  outline: none;
  color: #9DBFAF;
  background-color: rgba(23, 70, 143, 0.5);
}

.searchTerm:focus{
  color: #00B4CC;
}

.searchButton {
  width: 40px;
  height: 36px;
  border: 1px solid white;
  background: #17468f;
  text-align: center;
  color: #fff;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
  font-size: 20px;
}

/*Resize the wrap to see the search bar change!*/
.wrap{
  display:flex;
  width: 15%;
  flex-direction:row;
  justify-content: center;
  align-items: center;

}
body,
html {
    margin: 0;
    height: 100%;
    width: 100%;
    overflow: hidden;
}
</style>
