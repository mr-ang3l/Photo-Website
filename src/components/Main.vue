<script setup>
import { ref } from 'vue';
import Article from './Article.vue';
import S_Article from './ShortArticle.vue';

const fp_img_1 =
  'https://images.unsplash.com/photo-1682167176169-c74f2a6c6b84?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1916&q=80';

const fp_img_2 =
  'https://images.unsplash.com/photo-1695338035806-af02c934af38?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1964&q=80';

const fp_img_3 =
  'https://images.unsplash.com/photo-1695063536714-827da66eeb65?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2072&q=80';

const c1_img_1 =
  'https://images.unsplash.com/photo-1683009427042-e094996f9780?ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2071&q=80';

const c1_img_2 =
  'https://images.unsplash.com/photo-1682685797857-97de838c192e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80';

const c1_img_3 =
  'https://images.unsplash.com/photo-1695653422853-3d8f373fb434?ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80';

const c2_img_1 =
  'https://images.unsplash.com/photo-1675703236969-e4ce4d298618?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1928&q=80';

const c2_img_2 =
  'https://images.unsplash.com/photo-1695605117941-e9130a0369ad?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80';
</script>

<template>
  <h1 id="title">Best Of The Week</h1>
  <section id="frontP-wrapper">
    <div id="bigarticle">
      <Article class="item" title="Nathan Rogers" :source="fp_img_1" />
    </div>
    <div id="smallarticles">
      <S_Article class="item" title="Brock Wegner" :source="fp_img_2" />
      <S_Article class="item" title="Daniel Lee" :source="fp_img_3" />
    </div>
  </section>
  <h1 id="title">Recent Uploads</h1>
  <section id="art-wrapper">
    <div id="body_articles_column_1">
      <Article class="item" title="Daniel J. Schwarz" :source="c1_img_1" />
      <Article class="item" title="NEOM" :source="c1_img_2" />
      <Article class="item" title="Grab" :source="c1_img_3" />
    </div>
    <div id="body_articles_column_2">
      <Article class="item" title="Godefroy Chabanas" :source="c2_img_1" />
      <Article class="item" title="Greg Johnson" :source="c2_img_2" />
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=MuseoModerno:wght@500&display=swap');

#title {
  width: fit-content;
  margin: 1rem;
  margin-left: 0;
  padding: 0;
  padding-inline: 10px;
  font-size: 5em;
  text-align: start;
  background-color: #213547;
}

#frontP-wrapper {
  box-sizing: border-box;
  width: 1280px;
  max-height: 900x;
  margin: 0;
  margin-bottom: 50px;
  display: flex;
  flex-direction: row nowrap;
  justify-content: space-between;
  gap: 25px;
  color: white;
}

#bigarticle {
  box-sizing: border-box;
  width: 100%;
  height: 900px;
  margin: 0;
  padding: 0px;
}

#smallarticles {
  box-sizing: border-box;
  height: 900px;
  margin: 0;
  padding: 0;
  display: grid;
  grid-template-rows: 450px 450px;
  grid-template-columns: 620px;
}

.item {
  height: 100%;
}

#example {
  background-color: yellow;
}

#art-wrapper {
  box-sizing: border-box;
  width: 1280px;
  max-height: 100%;
  margin: 0;
  padding-bottom: 20px;
  gap: 25px;
  display: flex;
  flex-direction: row nowrap;
  color: white;
}

#body_articles_column_1 {
  box-sizing: border-box;
  width: 640px;
  margin: 0;
  padding: 0px;
  gap: 50px;
  display: flex;
  flex-direction: column;
}

#body_articles_column_2 {
  box-sizing: border-box;
  width: 640px;
  margin: 0;
  padding: 0px;
  gap: 50px;
  display: flex;
  flex-direction: column;
}

.item:hover {
  transition: all 500ms ease-out;
  cursor: pointer;
  transform: scale(0.95);
}
</style>
