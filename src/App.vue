<script setup>
import FrontPage from './components/FrontPage.vue';
import Main from './components/Main.vue';
</script>

<template>
  <div id="main">
      <h1 id="main-behind">윈도우즈</h1>
      <h1 id="main-title">윈도우즈</h1>
      <FrontPage />
      <Main />
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Gasoek+One&display=swap');

@import url('https://fonts.googleapis.com/css2?family=MuseoModerno:wght@500&display=swap');

  #main {
  }

  #main-behind {
    position: absolute;
    width: 1280px;
    top: -45px;
    text-align: center;
    z-index: -2;
    margin: 0;
    padding: 0;
    padding-bottom: .1em;
    font-family: Gasoek One;
    font-size: 20em;
    font-weight: bold;
    color: #003049;
    cursor: default;
    transition: all 200ms ease-out;
  }

  #main-title {
    margin: 0;
    padding: 0;
    padding-bottom: .1em;
    font-family: Gasoek One;
    font-size: 10em;
    font-weight: bold;
    color: #e63946;
    -webkit-text-stroke-width: 3px;
    -webkit-text-stroke-color: white;
    text-shadow: 4px 3px 6px rgba(0,0,0,0.57);
    transition: all 200ms ease-out;
    cursor: default;
  }

  #main-title:hover {
    transform: scale(1.05);
  }
</style>
