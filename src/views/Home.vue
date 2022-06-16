<template>
  <div class="home">
        <Navbar/>
      <div class="banner">
      <div class="first-part">
        <h1 class="safe-text mb-3">SAFETY</h1>
        <div class="box" style="background-color:blue;">
          <a href="">LEVEL 1</a>
        </div>
        <div class="box my-5" style="background-color:blue;">
          <a href="">LEVEL 1</a>
        </div>
        <div class="box" style="background-color:blue;">
          <a href="">LEVEL 1</a>
        </div>
      </div>
      <div class="second-part">hbd</div>
      </div>
  </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'

export default {
  name: 'Home',
  components : {
    Navbar
  }
}
</script>

<style lang="scss" scoped>
.banner{
  display: flex;
  height: calc(100vh - 74px);
}
.first-part{
  width: 50%;
  height: calc(100vh - 74px);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  background-color: red;
}
.second-part{
  width: 50%;
  height: calc(100vh - 74px);
  background-color: blue;
  display: flex;
  align-items: center;
  justify-content: center;
}
.box{
  padding: 20px 60px;
  border: none;
  cursor: pointer;
  outline: none;


  a{
    text-decoration: none;
    color: white;
    
  }
}
.safe-text{
  color: white;
  margin-bottom: 20px;
  font-size: 60px;
}
</style>
