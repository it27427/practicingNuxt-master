<template>
  <div class="row g-4">
    <div v-for="(doctor, i) in doctorInfoList" :key="i" class="col-lg-4 col-6">
      <DoctorCard :docinfo="doctor" />
    </div>
  </div>
</template>

<script>
import DoctorCard from '~/components/Cards/DoctorCard';

export default {
  name: 'AllDoc',
  components: {
    DoctorCard
  },

  data() {
    return {
      doctorInfoList: [
        {
          "id": "doctor-1",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "isActive": true
        },
        {
          "id": "doctor-2",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-3",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-4",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-5",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-6",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শরীফুল ইসলাম শরীফ",
          "designation": "ক্যান্সার, অর্থোসার্জারী ও প্লাষ্টিক সার্জারি বিশেষজ্ঞ",
          "isActive": false
        },
        {
          "id": "doctor-7",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ অমিত চন্দ্র দেব",
          "designation": "মেডিসিন, গ্যাষ্ট্রিক, লিভার, ডায়াবেটিস, বক্ষব্যাধি, মা ও শিশু রোগ বিশেষজ্ঞ এবং সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-8",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ শামছুর রহমান",
          "designation": "বিশেষজ্ঞ সার্জন",
          "isActive": false
        },
        {
          "id": "doctor-9",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ জোবাইদুল হক",
          "designation": "নাক, কান, গলা রোগ বিশেষজ্ঞ ও সার্জন",
          "isActive": true
        },
        {
          "id": "doctor-10",
          "imgSrc": "~/static/assets/images/doctors/doctor-thumbnail.png",
          "name": "ডাঃ মোঃ লুৎফর রহমান",
          "designation": "স্ত্রী রোগ ও প্রসূতিবিদ্যা বিশেষজ্ঞ এবং সার্জন",
          "isActive": false
        },
      ]
    }
  },
}
</script>
