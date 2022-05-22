<template>
  <div class="row g-5">
    <div class="col-lg-9 col-md-8 col-12">
      <DoctorGrid />
    </div>

    <div class="col-lg-3 col-md-4 col-12">
      <div class="categories">
        <Categories />

        <div class="seeall">
          <a href="#" class="seeall-link">See All</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Categories from '~/components/Categories/Categories';
import DoctorGrid from '~/components/DoctorGrid/DoctorGrid';

export default {
  name: 'DocInfo',
  components: {
    Categories,
    DoctorGrid
  }
}
</script>