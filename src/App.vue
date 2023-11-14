<template>
  <div>
    <greet name="Nay" heroName="Batman"></greet>
    <greet name="Zaw" heroName="Ant Man"></greet>
    <greet name="Aung" heroName="Super Man"></greet>
    <greet :name="name" :heroName="channel"></greet>
  </div>
</template>

<script>
import Greet from './components/Greet.vue';
export default {
  name: 'App',
  components: {
    Greet,
  },
  data(){
    return{
      name:'Na Na',
      channel:'Developer Nay',
    }
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
  margin-top: 60px;
}
</style>
