<template>
  <span>
    {{ day.name }}
  </span>
</template>

<script>
  export default {
    name: 'DayOption',
    props: {
      dayInfo: {
        type: Object,
        required: true
      }
    },
    computed: {
      day() {
        return this.$props.dayInfo
      }
    }
  }
</script>