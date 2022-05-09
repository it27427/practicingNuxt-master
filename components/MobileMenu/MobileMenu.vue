<template>
	<div id="mobileMenu" class="offcanvas offcanvas-start" tabindex="-1" aria-labelledby="mobileMenu">
		<div class="offcanvas-header">
			<nuxt-link to="/" class="logo">
				<img src="~/static/assets/images/logo/logo.png" alt="logo">
			</nuxt-link>

			<button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close">
				<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-left-circle" viewBox="0 0 16 16">
					<path fill-rule="evenodd" d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8zm15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-4.5-.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5H11.5z"/>
				</svg>
			</button>
		</div>
		
		<div class="offcanvas-body">
				<!-- MOBILE-LIST START -->
				<ul class="mobilelist">
					<li class="mobilelist-item">
						<nuxt-link to="/" class="mobilelist-link">Home</nuxt-link>
					</li>

					<li class="mobilelist-item">
						<nuxt-link to="/doctors" class="mobilelist-link">Doctors</nuxt-link>
					</li>

					<li class="mobilelist-item">
						<nuxt-link to="/hospital" class="mobilelist-link">Hospital</nuxt-link>
					</li>

					<li class="mobilelist-item">
						<nuxt-link to="/blog" class="mobilelist-link">Blog</nuxt-link>
					</li>
				</ul>
				<!-- MOBILE-LIST END -->
		</div>
	</div>
</template>

<script>
export default {
	name: 'MobileMenu'
}
</script>