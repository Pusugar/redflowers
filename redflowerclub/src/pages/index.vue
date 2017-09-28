<template>
  <div class="index wrapper">
    <section class="leftbox">
      <div class="flexbox">
        <div class="logobox">
          <img src="../assets/logo-white.png" alt="logo" class="logo" width="98" height="98">
          <h1> {{ enTittle }} </h1>
          <h1> {{ cnTittle }} </h1>
        </div>
        <div class="loginbox">
          <input type="text" name="" value="" placeholder="User">
          <input type="password" name="" value="" placeholder="Password">
          <button type="submit" name="button" class="loginbtn">Login</button>
        </div>
      </div>
    </section>
    <section class="rightbox">
      <div class="introbox">
        <p><b>红花会（RedFlowerClub）</b>，中国地下私募组织，致力于投资和慈善；</p>
        <p class="tips">暂不对外开放。</p>
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
      cnTittle: '红花会'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #FFF;
  font-size: 2.4rem;
  margin: 0 0 1rem 0;
  line-height: 2.4rem;
}

.logobox {
  margin: 80px 0;
}

.logo {
  margin-bottom: 1rem;
  transition: all 1s ease-in-out;
}

.logo:hover {
  transform: rotate(360deg);
}

.loginbox {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
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
  line-height: 4rem;
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

.rightbox .tips {
  font-size: 2.4rem;
  font-weight: bold;
  color: #E34C41;
  margin-top: 4rem;
}
</style>
