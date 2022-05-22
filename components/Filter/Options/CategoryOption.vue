<template>
  <span>
    {{ category.title }}
  </span>
</template>

<script>
  export default {
    name: 'CategoryOption',
    props: {
      ctgInfo: {
        type: Object,
        required: true
      }
    },
    computed: {
      category() {
        return this.$props.ctgInfo
      }
    }
  }
</script>