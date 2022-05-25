<template>
  <div class="card-gallery">
    <div class="card-gallery-header">
      <div class="card-thumbnail">
        <img src="~/static/assets/images/doctors/doctor-3.png" alt="doctor-thumbnail">
      </div>
    </div>
    
    <div class="card-gallery-body">
      <div class="doctorname">
        <p class="name">{{ doctor.name }}</p>
      </div>

      <div class="doctorpost">
        <p class="position">{{ doctor.designation }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'GalleryCard',
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