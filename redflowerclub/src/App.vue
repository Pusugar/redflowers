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
}

input, button {
  outline: none;
  border-radius: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #FFF;
}

.wrapper {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.leftbox, .rightbox{
  flex: 1;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.leftbox {
  background: #E34C41;
}

.rightbox {
  background: #FFF;
}

@media(max-width: 736px){
  .wrapper {
    flex-direction: column;
  }
  .leftbox, .rightbox {
    flex: auto;
  }
}

</style>
