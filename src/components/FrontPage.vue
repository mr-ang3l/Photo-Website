<script setup>
import { ref } from 'vue';

const id = ref('image-test');
</script>

<template>
  <section id="wrapper">
    <img
      id="front-page"
      src="https://images.unsplash.com/photo-1682687218904-de46ed992b58?ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2143&q=80"
    />
    <img
      id="image-test"
      src="https://images.unsplash.com/photo-1695597778289-fc1f5c715958?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2071&q=80"
    />
    <div id="front-gr"></div>
    <p>NEOM, Saudi Arabia</p>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=MuseoModerno:wght@500&display=swap');

@import url('https://fonts.googleapis.com/css2?family=Gasoek+One&display=swap');

  #wrapper {
    width: 1280px;
    height: 400px;
    border: white solid 0px;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    border-radius: 1em 1em 0 0;
  }

  #front-page {
    z-index: 1;
    width: 1280px;
    margin: 0;
    padding: 0;
    display: static;
    object-fit: cover;
    border-radius: 1em 1em 0 0;
  }

  #image-test {
    z-index: 2;
    width: 100%;
    height: 250px;
    margin: 0;
    padding: 0;
    position: absolute;
    display: none;
  }

  #front-gr {
    z-index: 3;
    height: 400px;
    width: 1280px;
    position: absolute;
    background-image: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0),
      rgba(0, 0, 0, 0),
      rgba(36, 36, 36, 0.025),
      rgba(36, 36, 36, 0.12),
      rgba(36, 36, 36, 1)
    );
  }

  p {
    height: 400px;
    width: 1280px;
    margin: 0;
    padding: 0;
    padding-right: .8em;
    z-index: 4;
    display: flex;
    align-items: end;
    justify-content: end;
    position: absolute;
    font-size: 2.5em;
    font-weight: bold;
    font-family: MuseoModerno;
  }
</style>
