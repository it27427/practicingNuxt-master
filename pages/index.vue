<template>
  <div>
    <div class="home-slider">
      <div class="container p-0">
        <div class="home-slider-content">
          <!-- HOME-SLIDER HEADER START -->
          <div class="home-slider-header">
            <div class="sliderinfo">
              <h1 class="slider-title">Today's Doctors</h1>
            </div>

            <div class="clockinfo">
              <p class="date">{{ currentDateTime() }}</p>
              <!-- <p class="time">{{ time }}</p> -->
            </div>
          </div>
          <!--- HOME-SLIDER HEADER END --->
          
          <!-- HOME-SLIDER BODY START -->
          <div class="home-slider-body">
            <SwiperSlider />
          </div>
          <!--- HOME-SLIDER BODY END --->
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import SwiperSlider from '~/components/Slider/SwiperSlider'

export default {
  name: 'IndexPage',
  components: {
    SwiperSlider
  },

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
