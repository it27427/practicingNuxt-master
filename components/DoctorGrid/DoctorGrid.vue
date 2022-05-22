<template>
  <div class="doctorgallery">
    <div class="gallery-info">
      <div class="gallery-details">
        <div v-for="(doctor, i) in doctorInfoList" :key="i" class="thumbitem">
          <GalleryCard :docinfo="doctor"/>
        </div>
      </div>
    </div>

    <div class="gallery-thumbs">
      <div v-for="(doc, i) in docInfoList" :key="i" class="item">
        <ThumbCard :info="doc" />
      </div>
    </div>
  </div>
</template>

<script>
import GalleryCard from '~/components/Cards/GalleryCard';
import ThumbCard from '~/components/Cards/ThumbCard';

export default {
  components: {
    GalleryCard,
    ThumbCard
  },

  data() {
    return {
      doctorInfoList: [
        {
          "id": "doctor-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ"
        }
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
  }
}
</script>