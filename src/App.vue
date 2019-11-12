<template>
  <div id="app">
    <Navigation />
    <Selection />
  </div>
</template>

<script>
import Navigation from "./components/nav.vue";
import Selection from "./components/selection.vue";
import booklist from './components/booklist.vue';
export default {
  
  name: "app",
  components: {
    Navigation,
    Selection
  },

  methods:{
   get: function() {
       console.log(booklist.props)
     }
 },
 beforeMount(){
    this.get()
 },
  data() {
    return { 
      }
  },
};
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
