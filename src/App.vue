<template>
  <div id="app">
    <div class="top">
      <div class="profile-image">
        <img src="" alt="">
      </div>
      <div class="top-credentials">
        <p>name</p>
        <p>email</p>
      </div>
    </div>
    <Main />
  </div>
</template>
<script>
import Main from './components/Main.vue'

export default{
  name: 'App',
  components: {
    Main,
  }
  
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
