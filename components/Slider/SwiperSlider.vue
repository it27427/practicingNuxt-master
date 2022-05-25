<template>
  <div class="container p-0">
    <div ref="swiper" class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div v-for="(doctor, i) in doctorInfoList" :key="i" class="swiper-slide">
          <DoctorCard :docinfo="doctor" />
        </div>
      </div>

      <!-- SLIDER-ARROWS START -->
      <button class="swiper-button-next">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-chevron-right" viewBox="0 0 16 16">
          <path fill-rule="evenodd" d="M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z"/>
        </svg>
      </button>

      <button class="swiper-button-prev">
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-chevron-left" viewBox="0 0 16 16">
          <path fill-rule="evenodd" d="M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z"/>
        </svg>
      </button>
      <!--- SLIDER-ARROWS END --->
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min';
import 'swiper/swiper-bundle.min.css';
import DoctorCard from '~/components/Cards/DoctorCard';

export default {
  components: {
    DoctorCard
  },

  data() {
    return {
      doctorInfoList: [
        {
          "id": "doctor-11",
          "imgSrc": "~/static/assets/images/doctors/doctor-11.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "isActive": true
        },
        {
          "id": "doctor-10",
          "imgSrc": "~/static/assets/images/doctors/doctor-10.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-9",
          "imgSrc": "~/static/assets/images/doctors/doctor-9.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-8",
          "imgSrc": "~/static/assets/images/doctors/doctor-8.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-7",
          "imgSrc": "~/static/assets/images/doctors/doctor-7.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-6",
          "imgSrc": "~/static/assets/images/doctors/doctor-6.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "isActive": false
        },
        {
          "id": "doctor-5",
          "imgSrc": "~/static/assets/images/doctors/doctor-5.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-4",
          "imgSrc": "~/static/assets/images/doctors/doctor-4.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-3",
          "imgSrc": "~/static/assets/images/doctors/doctor-3.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-2",
          "imgSrc": "~/static/assets/images/doctors/doctor-2.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-1.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "isActive": false
        }
      ]
    }
  },

  async mounted() {
    await this.$nextTick();
    new Swiper(this.$refs.swiper, {
      autoplay: true,
      autoplayDisableOnInteraction: false,
      speed: 1000,
      slidesPerView: 1,
      spaceBetween: 16,
      loop: true,
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      breakpoints: {
        360: {
          slidesPerView: 2
        },
        992: {
          slidesPerView: 3
        },
        1280: {
          slidesPerView: 4
        }
      }
    });
  },
}
</script>
