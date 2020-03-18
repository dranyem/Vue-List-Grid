<template>
  <div id="app">
    <Button/>
    <TweetList/>
  </div>
</template>

<script>
import Button from './components/Button.vue'
import TweetList from './components/TweetList.vue'
export default {
  name: 'App',
  components: {
    Button,
    TweetList
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
#app {
  display: grid;
  gap: 10px;
  place-items: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
