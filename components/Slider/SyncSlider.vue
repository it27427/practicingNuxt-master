<template>
  <div>
    <div class="sliderinfo">
        <div class="swiper-container gallery-top">
        <div class="swiper-wrapper">
          <div v-for="(doctor, i) in doctorInfoList" :key="i" class="swiper-slide">
            <div class="slider-details">
              <SliderCard :docinfo="doctor"/>
            </div>
          </div>
        </div>
      </div>

      <div class="swiper-container gallery-thumbs">
        <div class="swiper-wrapper">
          <div v-for="(doc, i) in docInfoList" :key="i" class="swiper-slide">
            <div class="slide-details">
              <SlideCard :info="doc" />
            </div>
          </div>
        </div>

        <!-- Add Arrows -->
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
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper/swiper-bundle.min';
import 'swiper/swiper-bundle.min.css';

import SliderCard from '~/components/Cards/SliderCard';
import SlideCard from '~/components/Cards/SlideCard';

export default {
components: {
  SliderCard,
  SlideCard
},

  data() {
    return {
      doctorInfoList: [
        {
          "id": "doctor-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ"
        },
        {
          "id": "doctor-2",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন"
        },
        {
          "id": "doctor-3",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন"
        },
        {
          "id": "doctor-4",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন"
        },
        {
          "id": "doctor-5",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন"
        },
        {
          "id": "doctor-6",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ"
        },
        {
          "id": "doctor-7",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন"
        },
        {
          "id": "doctor-8",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন"
        },
        {
          "id": "doctor-9",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন"
        },
        {
          "id": "doctor-10",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন"
        },
      ],

      docInfoList:  [
        {
          "id": "doc-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ"
        },
        {
          "id": "doc-2",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব"
        },
        {
          "id": "doc-3",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান"
        },
        {
          "id": "doc-4",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক"
        },
        {
          "id": "doc-5",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান"
        },
        {
          "id": "doc-6",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ"
        },
        {
          "id": "doc-7",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব"
        },
        {
          "id": "doc-8",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান"
        },
        {
          "id": "doc-9",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক"
        },
        {
          "id": "doc-10",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান"
        },
      ]
    }
  },

  async mounted() {
    await this.$nextTick();

    const galleryTop = new Swiper('.gallery-top', {
      loop: true,
      loopedSlides: 10,
      spaceBetween: 10
    });
    
    const galleryThumbs = new Swiper('.gallery-thumbs', {
      autoplay: true,
      loop: true,
      centeredSlides: true,
      spaceBetween: 8,
      slideToClickedSlide: true,
      watchSlidesVisibility: true,
      watchSlidesProgress: true,
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      breakpoints: {
        360: {
          slidesPerView: 2
        },
        768: {
          slidesPerView: 3
        },
        992: {
          slidesPerView: 4
        },
        1280: {
          slidesPerView: 5
        }
      }
    });


    // ALTERNATIVE SOLUTION to get the active thumb centered, it doesn't work on Safari if sliding backwards
    galleryTop.controller.control = galleryThumbs;
    galleryThumbs.controller.control = galleryTop;
  },
}
</script>