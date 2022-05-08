<template>
	<client-only>
		<div class="card-doctor">
			<div class="card-doctor-header">
				<img :src="docinfo.imgSrc" alt="doctor-thumbnail">
			</div>
			
			<div class="card-doctor-body">
				<div class="doctorname">
					<span class="name">{{ docinfo.name }}</span>
					<span :class="{ active: isActive }" class="status"></span>
				</div>

				<div class="doctorpost">
					<p class="position">Psychiatrist</p>
				</div>

				<div class="ragings">
					<p class="ratingtext">4.5</p>

					<ul class="ratinglist">
							<li class="ratinglist-item">
								<svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M8.12651 2.77007C8.38688 1.97073 9.51776 1.97073 9.77727 2.77007L10.7059 5.62722C10.7627 5.80122 10.873 5.95284 11.021 6.0604C11.1691 6.16795 11.3474 6.22594 11.5304 6.22608H14.5351C15.3761 6.22608 15.725 7.30228 15.0455 7.79699L12.6153 9.56231C12.4669 9.66996 12.3564 9.82182 12.2997 9.99614C12.2429 10.1704 12.2428 10.3583 12.2994 10.5326L13.2281 13.3898C13.4884 14.1891 12.5728 14.8548 11.8915 14.3601L9.46135 12.5948C9.31312 12.4872 9.13463 12.4292 8.95146 12.4292C8.76828 12.4292 8.58979 12.4872 8.44156 12.5948L6.01142 14.3601C5.33098 14.8548 4.41621 14.1891 4.67571 13.3898L5.60437 10.5326C5.66094 10.3583 5.66084 10.1704 5.60408 9.99614C5.54733 9.82182 5.43684 9.66996 5.28845 9.56231L2.85918 7.79786C2.17961 7.30315 2.52938 6.22694 3.36951 6.22694H6.37334C6.55651 6.22699 6.735 6.16909 6.88325 6.06152C7.03151 5.95395 7.14193 5.80223 7.19872 5.62809L8.12738 2.77094L8.12651 2.77007Z" fill="#F2B807"></path>
								</svg>
							</li>
							
							<li class="ratinglist-item">
								<svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M8.12651 2.77007C8.38688 1.97073 9.51776 1.97073 9.77727 2.77007L10.7059 5.62722C10.7627 5.80122 10.873 5.95284 11.021 6.0604C11.1691 6.16795 11.3474 6.22594 11.5304 6.22608H14.5351C15.3761 6.22608 15.725 7.30228 15.0455 7.79699L12.6153 9.56231C12.4669 9.66996 12.3564 9.82182 12.2997 9.99614C12.2429 10.1704 12.2428 10.3583 12.2994 10.5326L13.2281 13.3898C13.4884 14.1891 12.5728 14.8548 11.8915 14.3601L9.46135 12.5948C9.31312 12.4872 9.13463 12.4292 8.95146 12.4292C8.76828 12.4292 8.58979 12.4872 8.44156 12.5948L6.01142 14.3601C5.33098 14.8548 4.41621 14.1891 4.67571 13.3898L5.60437 10.5326C5.66094 10.3583 5.66084 10.1704 5.60408 9.99614C5.54733 9.82182 5.43684 9.66996 5.28845 9.56231L2.85918 7.79786C2.17961 7.30315 2.52938 6.22694 3.36951 6.22694H6.37334C6.55651 6.22699 6.735 6.16909 6.88325 6.06152C7.03151 5.95395 7.14193 5.80223 7.19872 5.62809L8.12738 2.77094L8.12651 2.77007Z" fill="#F2B807"></path>
								</svg>
							</li>
					</ul>
				</div>

				<div class="profilelink">
					<a href="#" class="link">
						Visit Profile -&gt;
					</a>
				</div>

				<div class="appointmentinfo">
					<a href="#" class="btn-appointmant">Get Appointment</a>
				</div>
			</div>
		</div>
	</client-only>
</template>

<script>

export default {
	name: 'Doctor',
	// props: ['docinfo'],
  // data() {
  //   return {
  //     // counter only uses this.docinfo as the initial value;
  //     // it is disconnected from future prop updates.
  //     counter: this.docinfo
  //   }
  // }
}
</script>