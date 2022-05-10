<template>
  <div class="row g-4">
    <div class="col-lg-9 col-md-8 col-12">

    </div>

    <div class="col-lg-3 col-md-4 col-12">
      <CategorySidebar/>
    </div>
  </div>
</template>

<script>
  import CategorySidebar from '~/components/CategorySidebar/CategorySidebar';

  export default {
    name: 'DocInfo',
    components: {
      CategorySidebar
    }
  }
</script>