<template>
  <div>
    <div class="card-slide">
      <div class="card-slide-header">
        <div class="card-thumbnail">
				  <img src="~/static/assets/images/doctors/doctor-thumbnail.png" alt="doctor-thumbnail">
        </div>
      </div>
      
      <div class="card-slide-body">
        <div class="doctorname">
				  <p class="name">{{ doc.name }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SlideCard',
	props: {
		info: {
			type: Object,
			required: true
		}
	},
	computed: {
		doc() {
			return this.$props.info
		}
	}
}
</script>