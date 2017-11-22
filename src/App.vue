<template>
  <div id="app">
    <div class="device-panel">
      <div class="device">
        <div class="screen" :style="{ backgroundImage: `url(${imageURI})` }" />
      </div>
    </div>
    <div class="controls">
      <input v-model="imageURI" type="text" placeholder="Image URI"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      imageURI: '',
      msg: 'Welcome to Your Vue.js App'
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
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


#app {
  display: flex;
  flex-flow: column;
  align-items: center;
}
.device {
  padding: 20px;
  border-radius: 5px;
  background: #ccc;
}

.screen {
  width: 400px;
  height: 400px;
  background: #000;
  background-size: cover;
  background-position: center;
}
</style>
