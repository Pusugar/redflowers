<template>
  <div class="hello">
    <h1>{{ enMsg }}</h1>
    <h1>{{ cnMsg }}</h1>
    <button class="espect-btn" type="button" name="button">敬请期待</button>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      enMsg: 'Welcome to Red Flower Club',
      cnMsg: '欢迎来到红花会'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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

.espect-btn {
  width: 120px;
  height: 60px;
  font-size: 18px;
  background: #fff;
  color: #e9002d;
  border: 3px solid #e9002d;
}
</style>
