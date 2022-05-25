<template>
  <div class="row g-4">
    <div class="col-lg-6 col-12">
      <div class="card-blog-thumbnail">
        <img :src="blog.imageSrc" alt="blog-thumbnail">
      </div>
    </div>

    <div class="col-lg-6 col-12">
      <div class="card-blog-details">
        <div class="info">
          <div class="info-head">
            <h1 class="blogtitle">{{ blog.title }}</h1>
            <p class="date">{{ blog.date }}</p>
          </div>

          <div class="info-body">
            <p class="blogtext">{{ blog.text }}</p>
          </div>
        </div>

        <div class="readinfo">
          <nuxt-link to="/blog-details" class="btn-read">{{ blog.linktext }}</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'BigBlog',
    props: {
      blogs: {
        type: Object,
        required: true
      }
    },
    computed: {
      blog() {
        return this.$props.blogs
      }
    }
  }
</script>