<template>
  <div class="container p-0">
    <div class="row g-4">
      <div v-for="(test, i) in testInfoList" :key="i" class="col-md-4 col-lg-3 col-6">
        <TestCard :test-info=test />
      </div>
    </div>
  </div>
</template>

<script>
import TestCard from '~/components/Cards/TestCard';

export default {
  name: 'Test',
  
  components: {
    TestCard
  },

  data() {
    return {
      testInfoList: [
        {
          "id": "test-1",
          "imgSrc": "~/static/assets/images/tests/test-1.jpg",
          "testName": "ABG"
        },
        {
          "id": "test-2",
          "imgSrc": "~/static/assets/images/tests/test-2.jpg",
          "testName": "ESR"
        },
        {
          "id": "test-3",
          "imgSrc": "~/static/assets/images/tests/test-3.jpg",
          "testName": "Colposcopy"
        },
        {
          "id": "test-4",
          "imgSrc": "~/static/assets/images/tests/test-4.jpg",
          "testName": "Xray"
        },
        {
          "id": "test-5",
          "imgSrc": "~/static/assets/images/tests/test-5.jpg",
          "testName": "Arthroscopy"
        },
        {
          "id": "test-6",
          "imgSrc": "~/static/assets/images/tests/test-1.jpg",
          "testName": "Ultrasonography "
        },
        {
          "id": "test-7",
          "imgSrc": "~/static/assets/images/tests/test-2.jpg",
          "testName": "CT scan"
        },
        {
          "id": "test-8",
          "imgSrc": "~/static/assets/images/tests/test-3.jpg",
          "testName": "Polysomnography"
        }
      ]
    }
  }
}
</script>
