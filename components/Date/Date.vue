<template>
  <div>
    <p class="date">{{ currentDateTime() }}</p>
  </div>
</template>

<script>
  export default {
    methods: {
      currentDateTime() {
        const days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
        const monthNames = ['January', 'February', 'March', 'April', 'May', 'June','July', 'August', 'September', 'October', 'November', 'December'];
        const current = new Date();
        const day = new Date();
        const dayName = days[day.getDay()] + ',';
        
        const monthName = monthNames[day.getMonth()];

        const date = current.getDate() + ' ' + monthName + ' ' + current.getFullYear();

        const dateTime = dayName + ' ' + date;

        return dateTime;
      }
    }
  }
</script>