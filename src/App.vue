<template>
  <div id="app">
    <div class="d-flex app-container">
      <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
      <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
      <Sidebar />
      <div class="center">
        <div class="d-flex top-side">
          <form class="input-fr">
            <input type="text" class="form-control" />
          </form>
          <div class="right d-flex">
            <img src="./assets/icons/notification.png" class="notification"/>
            <div class="c">
              <span class="n">Ukauwa David</span><br />
              <span class="g">ukauwa@gmail.com</span>
            </div>
            <div>
              <img src="./assets/icons/user-profile.png" />
            </div>
          </div>
        </div>
        <StuFees />
        <div class="d-flex ss">
          <Perf />
          <Stats />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Navbar from './components/Navbar.vue'
import Sidebar from  './components/Sidebar.vue'
import StuFees from './components/StuFees.vue'
import Perf from './components/Perf.vue'
import Stats from './components/Stats.vue'

export default {
  name: 'app',
  components: {
    // HelloWorld
    Sidebar,
    StuFees,
    Perf,
    Stats
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
.app-container {
}
.center {
  padding-top: 17px;
  padding-left: 27px;
  padding-right: 27px;
  overflow: auto;
}
.top-side, .ss {
  overflow: auto;
}
.ss {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 20px;
}
.input-fr input{
  width: 50vw;
  height: 38px;
  background: url(./assets/icons/search.png) no-repeat scroll 13px 9px;
  background-color: #FFF;
  border: 1px solid rgba(189, 189, 189, 0.25);
  box-shadow: 0px 2px 9px rgba(196, 196, 196, 0.11);
}
.right {
  margin-left: 96px;
  margin-top: 8px;
}
.right .notification {
  width: 23px;
  height: 24px;
  margin-right: 25px;
}
.right .n {
  font-family: Khula;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  color: #31393C;
}
.right .g {
  font-family: Avenir Next;
  font-size: 9px;
  font-style: italic;
  color: #90A4AE;
}
.right .c {
  text-align: right;
  margin-right: 17px;
}
</style>
