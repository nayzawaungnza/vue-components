<template>
  <div>
    <!-- <greet name="Nay" heroName="Batman"></greet>
    <greet name="Zaw" heroName="Ant Man"></greet>
    <greet name="Aung" heroName="Super Man"></greet>
    <greet :name="name" :heroName="channel"></greet>
    <Article id="my-article" title="Article Title" :likes="50" :isPublished="true" /> -->
      <!-- <h3>AppComponent Username {{ name }}</h3>
    <ComponentC /> -->
    <button @click="showPopup = true">show</button>
    <Popup v-show="showPopup" @close="closePopup" />
  </div>
</template>

<script>
//import Greet from './components/Greet.vue';
//import Article from './components/Article.vue';
//import ComponentC from './components/ComponentC.vue';
import Popup from './components/Popup.vue';
export default {
  name: 'App',
  components: {
    //Greet,
    //Article,
    //ComponentC,
    Popup,
  },
  data(){
    return{
      showPopup:false,
       //name:'Na Na',
      // channel:'Developer Nay',
    }
  },
  methods:{
    closePopup(name){
      this.showPopup = false,
      console.log('Name', name);
    }
  },
  provide(){
    return{
      //username:this.name
    }
  },
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
