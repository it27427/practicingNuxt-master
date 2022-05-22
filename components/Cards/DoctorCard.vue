<template>
	<div class="card-doctor">
		<div class="card-doctor-header">
			<div class="card-thumbnail">
				<!-- <img :src="doctor.imgSrc ? doctor.imgSrc : '~/static/assets/images/doctors/doctor-thumbnail.png'" alt="doctor-thumbnail"> -->
				<img src="~/static/assets/images/doctors/doctor-thumbnail.png" alt="doctor-thumbnail">
			</div>
		</div>
		
		<div class="card-doctor-body">
			<div class="doctorname">
				<div class="naminfo">
					<span class="name">{{ doctor.name }}</span>
				</div>
				<span :class="{ 'active': doctor.isActive }" class="status d-none"></span>
			</div>

			<div class="doctorpost">
				<p class="position">{{ doctor.designation }}</p>
			</div>
		</div>
	</div>
</template>

<script>

export default {
	name: 'DoctorCard',
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