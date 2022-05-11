<template>
  <div>
    <div class="card-slider">
      <div class="card-slider-header">
        <div class="card-thumbnail">
				  <img src="~/static/assets/images/doctors/doctor-thumbnail.png" alt="doctor-thumbnail">
        </div>
      </div>
      
      <div class="card-slider-body">
        <div class="doctorname">
				  <p class="name">{{ doctor.name }}</p>
        </div>

        <div class="doctorpost">
          <p class="position">{{ doctor.designation }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SliderCard',
	props: {
		docinfo: {
			type: Object,
			required: true
		}
	},
	computed: {
		doctor() {
			return this.$props.docinfo
		}
	}
}
</script>