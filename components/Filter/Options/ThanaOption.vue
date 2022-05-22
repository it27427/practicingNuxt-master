<template>
  <span>
    {{ thana.name }}
  </span>
</template>

<script>
  export default {
    name: 'ThanaOption',
    props: {
      thanaInfo: {
        type: Object,
        required: true
      }
    },
    computed: {
      thana() {
        return this.$props.thanaInfo
      }
    }
  }
</script>