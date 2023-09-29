<script setup>
import { ref } from 'vue';

const props = defineProps({
  title: {
    type: String,
    default: 'no title',
  },
  likes: {
    type: Number,
    required: false,
  },
  source: {
    type: String,
    required: true,
    default: 'https://dinahosting.com/blog/upload/2021/03/error-404.jpg',
  },
});

const s = ref(props.source);
</script>

<template>
  <a :href='s' id="wrapper-art" target='blank'>
    <div id="img-container">
      <img id="img-art" :src="s" />
    </div>
    <h1 id="main-title">{{ title }}</h1>
  </a>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=MuseoModerno:wght@500&display=swap');

#wrapper-art {
  box-sizing: border-box;
  height: 100%;
  margin: 0;
  padding: 0;
  display: grid;
  grid-template-columns: 100%;
  grid-template-rows: 90% 10%;
  transition: all 500ms ease-out;
}

#img-container {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  background: pink;
}

#img-art {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

#main-title {
  margin: 0;
  margin-top: 10px;
  padding: 0;
  padding-left: 5px;
  display: flex;
  justify-content: start;
  align-items: center;
  font-size: 1.5em;
  font-family: MuseoModerno;
  background-color: whitesmoke;
  color: black;
}
</style>
