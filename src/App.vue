<template>
  <div id="app"  style="text-align:center;background-color:rgb(173,172,172);">
    <h1 class="text-center text-white" style="font-family:'Aguafina Script', cursive;">Single File Component Vue Applications.</h1>
    
    <div class="container">
         <CalenderWeek/>
        <CalenderEntry/>
          
    </div>
    <div>
      <CalenderFooter/> 
      </div>
    </div>
  <!-- </div> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

import CalenderWeek from './components/CalenderWeek.vue';
import CalenderEntry from './components/CalenderEntry.vue';
import CalenderFooter from './components/CalenderFooter.vue'
export default {
  name: 'app',
  components: {
    // HellCalenderoWorld
    CalenderEntry,
    CalenderWeek,
    CalenderFooter
  }
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
