<template>
  <div id="app">
    <div class="content">
      <div class="top">
        <div class="profile-image">
          <img src= "./assets/avataaars.png"  class="avatar" alt="avatars">
        </div>
        <div class="top-credentials">
          <p>name</p>
          <p>email</p>
        </div>
      </div>
      <Main />
    </div>
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


<style lang="sass" scoped>
.content
  display: flex
  align-items: center
  justify-content: center
  flex-direction: column
.top
  display: flex
  align-content: center
  justify-content: center
  align-items: center
  margin: 20px 0

.avatar    
  width: 80px
  height: 80px

.top-credentials
  p
    margin: 0

</style>
