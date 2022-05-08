<template>
  <div class="container p-0">
    <div ref="swiper" class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <DoctorCard :docinfo="doctorInfo" />
        </div>
      </div>
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min'
import 'swiper/swiper-bundle.min.css'
import DoctorCard from '~/components/cards/DoctorCard'

export default {
  components: {
    DoctorCard
  },

  data() {
    return {
      doctorInfo: [
        {
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "id": "doctor-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 4.5,
        },
        {
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "id": "doctor-2",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": false,
          "rating": 5,
        },
        {
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "id": "doctor-3",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 5,
        },
        {
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "id": "doctor-4",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": false,
          "rating": 4.5,
        },
        {
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "id": "doctor-5",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 4.5,
        },
        {
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "id": "doctor-6",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 4.5,
        },
        {
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "id": "doctor-7",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": false,
          "rating": 5,
        },
        {
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "id": "doctor-8",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 5,
        },
        {
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "id": "doctor-9",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": false,
          "rating": 4.5,
        },
        {
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "id": "doctor-10",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "isActive": true,
          "rating": 4.5,
        },
      ]
    }
  },

  async mounted() {
    await this.$nextTick();
    new Swiper(this.$refs.swiper, {
      slidesPerView: 5,
      spaceBetween: 30,
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
    });
  },
}
</script>
