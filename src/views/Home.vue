<template>
  <div class="home">
        <Navbar/>
      <div class="banner">
      <div class="first-part">
        <div class="AY">
        <h1 class="safe-text mb-3">HEALTH</h1>
        <div class="box" style="background-color:pink;">
          <a href="" style = "color:#111; font-weight:bold;">LEVEL 1</a>
        </div>
        <div class="box my-5" style="background-color:rgb(238, 83, 109);">
          <a href="" style = "color:#fff; font-weight:bold;">LEVEL 2</a>
        </div>
        <!-- <div class="box" style="background-color:pink;">
          <a href="" style = "color:#111; font-weight:bold;">LEVEL 3</a>
        </div> -->
        </div>
      </div>
      <div class="second-part">
        <div class="AY">
        <h1 class="safe-text mb-3">SAFETY</h1>
        <div class="box" style="background-color:cornflowerblue;">
          <a href="" style = "color:#fff; font-weight:bold;">LEVEL 1</a>
        </div>
        <div class="box my-5" style="background-color:rgb(14, 54, 128);">
          <a href="" style = "color:#fff; font-weight:bold">LEVEL 2</a>
        </div>
        <!-- <div class="box" style="background-color:cornflowerblue;">
          <a href="" style = "color:#fff; font-weight:bold">LEVEL 3</a>
        </div> -->
      </div>
      </div>
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
  background-repeat: no-repeat;
  background-attachment: fixed;
  flex-direction: column;
  background-size: cover;
  background-position: center;
  justify-content: center;
  // background: linear-gradient();
  // background-color: rgb(246, 176, 188);
  background-image: url('../assets/f.jpg'), linear-gradient(rgba(246, 176, 188),rgba(246, 176, 188));
}
.second-part{
  width: 50%;
  height: calc(100vh - 74px);
  // background-color: cornflowerblue;
  // background-color: rgb(103, 103, 183);
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: url('../assets/e.jpg');
  background-size: cover;
  background-position: center;
  flex-direction: column;

}
.box{
  padding: 30px 60px;
  border: none;
  cursor: pointer;
  border-radius: 20px;
  // color: rgb(14, 54, 128);
  outline: none;


  a{
    text-decoration: none;
    color: white;
    text-align: center;
  }
}
.AY{
  width: 50%;
  padding: 100px;
  opacity: .9;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  background-color: #111;
  border-radius: 30px;
}
.safe-text{
  color: #fff;
  margin-bottom: 20px;
  font-size: 50px;

  &::after{
    content: '';
    width: 50px;
    height: 3px;
    display: block;
    background-color: white;
    margin: 10px auto;
  }
}
@media (max-width:1200px){
  .safe-text{
    font-size: 35px;
  }
  .box{
    padding: 8px 20px;

  }
  .AY{
  
    .box{
      a{
        padding: 10px;
        text-align: center;
        display: inline-block;
      }
    }
  }
}

</style>
