<template>
  <div class="home">
    <!--<HelloWorld msg="Welcome to Your Vue.js App" />-->
    <div class="headerimage">
      <p>hello</p>
    </div>
    <div id="backshape">
      <div class="wrapper"></div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'Home',
  components: {
    //HelloWorld,
  },
};
</script>

<style scoped>
* {
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}

body {
  margin: 0;
}

@font-face {
  font-family: 'walsheim';
  src: url('../assets/GT-Walsheim-Regular.otf');
}

.headerimage {
  background-color: #083d08;
  height: 600px;
  width: 100%;
  background-size: cover;
  position: relative;
  z-index: -1;
  color: #fff;
  font-size: 40px;
  font-family: 'walsheim';
}

#backshape .wrapper {
  display: block;
  float: left;
  margin: 50px auto 200px;
  width: 100%;
  padding: 0 5%;
  transform: skew(0deg, -5deg);
  -ms-transform: skew(0deg, -10deg);
  -webkit-transform: skew(0deg, -5deg);
}

#backshape {
  z-index: 1;
  display: block;
  float: left;
  margin-top: -100px;
  width: 100%;
  background: white;
  transform: skew(0deg, 10deg);
  -ms-transform: skew(0deg, 10deg); /* IE 9 */
  -webkit-transform: skew(0deg, 5deg); /* Safari and Chrome */
}
</style>
