<template>
  <div id="app">
    <!-- <img class="logo" src="./assets/logo.png"> -->
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
* {
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
  font-size: 10px
}

html, body, .wrapper, .leftbox, .rightbox {
  min-height: 100vh;
  height: 100vh;
}

input, button {
  outline: none;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #FFF;
  min-height: 100%;
}

.wrapper {
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: center;
}

.leftbox {
  flex: 1;
  background: #E34C41;
}

.rightbox {
  flex: 1;
  background: #FFF;
  display: flex;
  flex-direction: column;
  align-self: center;
  align-items: center;
  justify-content: center;

}

</style>
