<template>
  <span>
    {{ district.name }}
  </span>
</template>

<script>
  export default {
    name: 'DistrictOption',
    props: {
      dtsInfo: {
        type: Object,
        required: true
      }
    },
    computed: {
      district() {
        return this.$props.dtsInfo
      }
    }
  }
</script>