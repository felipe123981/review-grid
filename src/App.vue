<template>
  <div id="app">
    <div class="catalog">
    <div v-for="i in 3" :key="i" :id="i">
      <Comment :cid="i"></Comment>
    </div>
  </div>
  </div>
</template>

<script>
import Comment from './components/CommentComponent.vue'

export default {
  name: 'App',
  components: {
    Comment
  }
}
</script>

<style>
#app {
  background-color: #e4e9f7;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.catalog {
      /* From https://css.glass */
background: rgba(255, 255, 255, 0.07);
border-radius: 16px;
box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
backdrop-filter: blur(1.7px);
-webkit-backdrop-filter: blur(1.7px);
border: 1px solid rgba(255, 255, 255, 0.25);
overflow-y: scroll;
height: 490px;
padding: 2px;
  /*
            height: 490px;
            overflow-y: scroll;
            
            border-radius: 16px;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
            
            padding: 5px;
            background-color: var(--body-color);
        */
          }
</style>
