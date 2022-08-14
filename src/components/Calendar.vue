<template>
  <div>
    <h1>Calendário Em Vue.Js </h1>

    <p>Data de reserva</p>
    <b-calendar v-model="value" :min="min" :max="max" locale="pt" 
        ></b-calendar>
  </div>
</template>

<script>
  export default {
    data() {
      const now = new Date()
      const today = new Date(now.getFullYear(), now.getMonth(), now.getDate())
      // 15th two months prior
      const minDate = new Date(today)
      minDate.setMonth(minDate.getMonth() )
      minDate.setDate(1)
      // 15th in two months
      const maxDate = new Date(today)
      maxDate.setMonth(maxDate.getMonth() )
      maxDate.setDate(5)

      return {
        value: '',
        min: minDate,
        max: maxDate
      }
    },
      methods: {
    
    }
  }
</script>

<style>
.b-calendar {
    margin-top: 10vh;
    margin-bottom: 10vh;
}
</style>
