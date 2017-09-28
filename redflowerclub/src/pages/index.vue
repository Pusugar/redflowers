<template>
  <div class="index wrapper">
    <section class="leftbox">
      <div class="logobox">
        <div class="logo">
          <img src="../assets/logo-white.png" alt="logo" width="98" height="98">
        </div>
        <h2> {{ enTittle }} </h2>
        <h1> {{ cnTittle }} </h1>
      </div>
      <div class="loginbox">
        <input type="text" name="" value="" placeholder="User">
        <input type="password" name="" value="" placeholder="Password">
        <button type="submit" name="button" class="loginbtn">Login</button>
      </div>
    </section>
    <section class="rightbox">
      <div class="introbox">
        <p><b>{{cnTittle}}（{{enTittle}}）</b>，{{intro}}；</p>
        <p class="notice">{{notice}}</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'index',
  data () {
    return {
      enTittle: 'Red Flower Club',
      cnTittle: '红花会',
      intro: '中国地下私募组织，致力于投资和慈善',
      notice: '暂不对外开放'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2{
  color: #FFF;
  margin: 0 0 1rem 0;
}

h1 {
  font-size: 4.2rem;
}

h2 {
  font-size: 2.4rem;
}

.logobox, .loginbox {
  width: 100%;
  flex: 1;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.logo img {
  margin-bottom: 1rem;
  transition: all 1s ease-in-out;
}

.logo img:hover {
  transform: rotate(360deg);
}

input {
  background: transparent;
  border-width: 0 0 1px 0;
  border-color: #FFF;
  padding-left: 2rem;
  width: 50%;
  line-height: 4rem;
  margin-bottom: 3rem;
  color: #FFF;
  font-size: 1.8rem;
}

input::placeholder {
  font-size: 1.8rem;
  color: rgba(255,255,255,0.8);
}

.loginbtn {
  color: #FFF;
  background: transparent;
  border: 1px solid #FFF;
  line-height: 4.8rem;
  width: 50%;
  margin-top: 2rem;
  font-size: 1.8rem;
}

.introbox {
  width: 60%;
  height: 300px;
  padding: 2rem;
  border: 3px solid #E34C41;
}

.rightbox p{
  color: #333;
  font-size: 1.8rem;
}

.rightbox .notice {
  font-size: 2.4rem;
  font-weight: bold;
  color: #E34C41;
  margin-top: 4rem;
}

@media(max-width: 736px){
  input, .loginbtn{
    width: 70%
  }
}
</style>
