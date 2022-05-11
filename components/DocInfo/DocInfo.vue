<template>
  <div class="row g-5">
    <div class="col-lg-9 col-md-8 col-12">
      <SyncSlider/>
    </div>

    <div class="col-lg-3 col-md-4 col-12">
      <CategorySidebar/>
    </div>
  </div>
</template>

<script>
import CategorySidebar from '~/components/CategorySidebar/CategorySidebar';
import SyncSlider from '~/components/Slider/SyncSlider';

export default {
  name: 'DocInfo',
  components: {
    CategorySidebar,
    SyncSlider,
  }
}
</script>