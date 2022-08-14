<template>
  <div id="app">
    <Calendar />
    <CalendarDatepicker />
  </div>
</template>

<script>
import Calendar from './components/Calendar.vue'
import CalendarDatepicker from './components/CalendarDatepicker.vue'

export default {
  name: 'App',
  components: {
    Calendar, CalendarDatepicker
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
  margin-right: 15vw;
  margin-left: 15vw; 
 
}

body {
 background-color: #8EC5FC;
background-image: linear-gradient(62deg, #8EC5FC 0%, #E0C3FC 100%);

}
</style>
