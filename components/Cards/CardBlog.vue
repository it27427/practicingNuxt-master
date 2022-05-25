<template>
  <nuxt-link to="/blog-details" class="bloglink">
    <div v-if="blogsingle !== {}" class="card-article">
      <div class="card-article-header">
        <img :src="blogsingle.imageSrc" alt="card-thumbnail">
      </div>

      <div class="card-article-body">
        <div class="title-date">
          <h4 class="title">{{ blogsingle.title }}</h4>
          <p class="date">{{ blogsingle.date }}</p>
        </div>

        <div class="articledescript">
          <p class="articletext">{{ blogsingle.text }}</p>
        </div>

        <span class="articlelink">{{ blogsingle.linktext }} -&gt;</span>
      </div>
    </div>
  </nuxt-link>
</template>

<script>
  export default {
    name: 'CardBlog',
    props: {
      blogs: {
        type: Object,
        required: true
      }
    },
    computed: {
      blogsingle() {
        return this.$props.blogs
      }
    }
  }
</script>