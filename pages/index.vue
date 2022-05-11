<template>
	<client-only>
    <div>
      <!-- HOME-SLIDER SECTION START -->
      <div class="home-slider">
        <div class="container p-0">
          <div class="home-slider-content">
            <!-- HOME-SLIDER HEADER START -->
            <header class="home-slider-header">
              <div class="sliderinfo">
                <h1 class="slider-title">Today's Doctors</h1>
              </div>

              <div class="clockinfo">
                <Date/>
              </div>
            </header>
            <!--- HOME-SLIDER HEADER END --->
            
            <!-- HOME-SLIDER BODY START -->
            <div class="home-slider-body">
              <SwiperSlider />
            </div>
            <!--- HOME-SLIDER BODY END --->
          </div>
        </div>

      </div>
      <!--- HOME-SLIDER SECTION END --->

      <!-- TEST SECTION START -->
      <section class="testsection">
        <div class="container">
          <div class="testsection-content">
            <header class="testsection-header">
              <h1 class="test-title">Tests</h1>
            </header>
            
            <div class="testsection-body">
              <Test/>
            </div>
          </div>
        </div>
      </section>
      <!--- TEST SECTION END --->

      <!-- BLOG-SECTION START -->
      <section class="blog">
        <div class="container">
          <div class="blog-content">
            <div class="blog-header">
              <h1 class="blog-title">Blogs</h1>
            </div>
            
            <div class="blog-body">
              <BlogGrid/>
            </div>
          </div>
        </div>
      </section>
      <!--- BLOG-SECTION END --->

      <!-- DOCTORSINFO-SECTION START -->
      <section class="doctorsinfo">
        <div class="container p-0">
          <div class="doctorsinfo-content">
            <div class="doctorsinfo-header">
              <h1 class="doctorsinfo-title">Doctors List</h1>
            </div>

            <div class="doctorsinfo-body">
              <DocInfo/>
            </div>
          </div>
        </div>
      </section>
      <!--- DOCTORSINFO-SECTION END --->
    </div>
	</client-only>
</template>

<script>
import SwiperSlider from '~/components/Slider/SwiperSlider';
import Test from '~/components/Test/Test';
import Date from '~/components/Date/Date';
import BlogGrid from '~/components/BlogGrid/BlogGrid';
import DocInfo from '~/components/DocInfo/DocInfo';

export default {
  name: 'IndexPage',
  components: {
    SwiperSlider,
    Test,
    Date,
    BlogGrid,
    DocInfo,
  },
  // mounted() {
  //   if(process.client) {
  //     if(document.querySelector('#mobileMenu') !== null && document.querySelector('#mobileMenu') !== undefined) {
  //       document.querySelector('#mobileMenu').offcanvas('hide');
  //     }
  //   }
  // }
}
</script>
