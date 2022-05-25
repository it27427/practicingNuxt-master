<template>
  <div class="card-thumb">
    <div class="card-thumb-header">
      <div class="card-thumbnail">
        <img src="~/static/assets/images/doctors/doctor-1.png" alt="doctor-thumbnail">
      </div>
    </div>
    
    <div class="card-thumb-body">
      <div class="doctorname">
        <p class="name">{{ doc.name }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ThumbCard',
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