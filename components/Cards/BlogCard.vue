<template>
  <div v-if="blog !== {}" class="card-blog" :class="blog.boxSize">
      <div class="card-blog-header">
        <img src="https://images.unsplash.com/photo-1470124182917-cc6e71b22ecc?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=" alt="test-thumbnail">
      </div>

      <div class="card-blog-body">
        <h6 class="card-blog-title">{{ blog.title }}</h6>
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