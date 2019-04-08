<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <ul>
      <li>
        <a href="#">1</a>
      </li>
      <li>
        <a href="#" class="active">2</a>
      </li>
      <li>
        <a href="#">3</a>
      </li>
      <li>
        <a href="#">4</a>
      </li>
    </ul>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style lang='less'>
html {
  font-size: 100px;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html,
body,
#app {
  height: 100%;
}

li:has(> a.active) {
  color: red;
}
</style>
