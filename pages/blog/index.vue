<template>
	<client-only>
    <main>
      <BlogBanner/>
      <Blog/>
      <BlogDescription/>
      <AllBlogs/>
    </main>
	</client-only>
</template>

<script>
  import BlogBanner from '~/components/BlogBanner/BlogBanner';
  import Blog from '~/components/Blog/Blog';
  import BlogDescription from '~/components/BlogDescription/BlogDescription';
  import AllBlogs from '~/components/AllBlogs/AllBlogs';

  export default {
    name: 'BlogPage',
    components: {
      BlogBanner,
      Blog,
      BlogDescription,
      AllBlogs
    }
  }
</script>
