<template>
  <div class="doctordetails">
    <DoctorDetails/>

    <div class="moredoc">
      <div class="moredoc-header py-4">
        <div class="container">
          <h4 class="title">Suggested Doctors</h4>
        </div>
      </div>
      <div class="moredoc-body">
        <SwiperSlider/>
      </div>
    </div>
  </div>
</template>

<script>
  import DoctorDetails from '~/components/DoctorDetails/DoctorDetails';


  import SwiperSlider from '~/components/Slider/SwiperSlider';

  export default {
    components: {
      SwiperSlider,
      DoctorDetails
    }
  }
</script>