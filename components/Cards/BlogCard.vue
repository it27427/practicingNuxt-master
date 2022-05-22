<template>
  <div v-if="blog !== {}" class="card-blog" :class="blog.boxSize">
      <div class="card-blog-header">
        <img src="https://images.unsplash.com/photo-1470124182917-cc6e71b22ecc?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=" alt="blog-thumbnail">
      
        <div class="bloginfo">
					<h6 class="card-blog-title">{{ blog.title }}</h6>

					<div class="details">
						<span class="author">
							<span class="icon">
								<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-person" viewBox="0 0 16 16">
									<path d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z"/>
								</svg>
							</span>
							<span class="author-name">{{ blog.author }}</span>
						</span>

						<span class="date">
							<span class="icon">
								<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-clock" viewBox="0 0 16 16">
									<path d="M8 3.5a.5.5 0 0 0-1 0V9a.5.5 0 0 0 .252.434l3.5 2a.5.5 0 0 0 .496-.868L8 8.71V3.5z"/>
									<path d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zm7-8A7 7 0 1 1 1 8a7 7 0 0 1 14 0z"/>
								</svg>
							</span>
							<span class="date-text">{{ blog.date }}</span>
						</span>
					</div>
				</div>

				<div class="overlay"></div>
			</div>
  </div>
</template>

<script>

export default {
	name: 'BlogCard',
	props: {
		blogInfo: {
			type: Object,
			required: true
		}
	},
	computed: {
		blog() {
			return this.$props.blogInfo
		}
	}
}
</script>