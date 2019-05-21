<template>
  <div id="app">
  <Avatars :msg="msg" :data="avatarsData"/> 
  </div>
</template>

<script>
import Avatars from './components/Avatar.vue'

export default {
  name: 'app',
  components: {
    Avatars
  },

  data() {
    return {
      msg : 'Avatars!!!',
      avatarsData: [
        {
          title:'Pavel',
          img:'logo.png',
          isActive : true
        },
        {
          title:'Dina',
          img:'logo.png',
          isActive : false
        },
        {
          title:'Lev',
          img:'logo.png',
          isActive : false
        },
      ]
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
