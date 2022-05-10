<template>
  <div v-if="test !== {}" class="card-test">
    <div class="card-test-header">
      <div class="card-thumbnail">
        <!-- <img :src="doctor.imgSrc ? doctor.imgSrc : '~/static/assets/images/tests/test-1.jpg'" alt="doctor-thumbnail"> -->
        <img src="~/static/assets/images/tests/test-1.jpg" alt="test-thumbnail">
      </div>
    </div>
    
    <div class="card-test-body">
      <h6 class="testname">{{ test.testName }}</h6>
    </div>
  </div>
</template>

<script>

export default {
	name: 'TestCard',
	props: {
		testInfo: {
			type: Object,
			required: true
		}
	},
	computed: {
		test() {
			return this.$props.testInfo
		}
	}
}
</script>