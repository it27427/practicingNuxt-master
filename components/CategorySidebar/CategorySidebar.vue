<template>
  <a href="#" class="sidebarlist-link">
    <span class="categorytitle">{{ category.title }}</span>
    <span class="categorycounter">({{ category.counter }})</span>
  </a>
</template>

<script>
  export default {
    name: 'CategorySidebar',
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