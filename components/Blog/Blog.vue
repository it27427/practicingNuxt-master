<template>
  <!--========== BLOG-SECTION START ==========-->
  <section class="blog">
    <div class="container">
      <div class="row g-lg-4 g-3">
        <!-- BLOG ITEM START -->
        <div v-for="(blog, i) in blogList" :key="i" class="col-lg-3 col-md-6 col-sm-6 col-10 mx-auto mx-lg-0">
          <CardBlog :blogs=blog />
        </div>
        <!-- BLOG ITEM END -->
      </div>
    </div>
  </section>
  <!--========== BLOG-SECTION END ============-->
</template>

<script>
  import CardBlog from '~/components/Cards/CardBlog';

  export default {
    name: 'Blog',
    components: {
      CardBlog
    },
    data() {
      return {
        blogList: [
          {
            imageSrc: 'https://images.unsplash.com/photo-1501183007986-d0d080b147f9?crop=entropy&cs=tinysrgb&fm=jpg&ixlib=rb-1.2.1&q=60&raw_url=true&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8ZnJlZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500',
            title: 'Blog Title 1',
            date: 'Wednesday May 25, 2022',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare pretium placerat ut platea...',
            linktext: 'Read article'
          },
          {
            imageSrc: 'https://images.unsplash.com/photo-1490730141103-6cac27aaab94?crop=entropy&cs=tinysrgb&fm=jpg&ixlib=rb-1.2.1&q=60&raw_url=true&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8ZnJlZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500',
            title: 'Blog Title 2',
            date: 'Wednesday May 25, 2022',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare pretium placerat ut platea...',
            linktext: 'Read article'
          },
          {
            imageSrc: 'https://images.unsplash.com/photo-1453060590797-2d5f419b54cb?crop=entropy&cs=tinysrgb&fm=jpg&ixlib=rb-1.2.1&q=60&raw_url=true&ixid=MnwxMjA3fDB8MHxzZWFyY2h8OXx8ZnJlZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500',
            title: 'Blog Title 3',
            date: 'Wednesday May 25, 2022',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare pretium placerat ut platea...',
            linktext: 'Read article'
          },
          {
            imageSrc: 'https://images.unsplash.com/photo-1507835661088-ac1e84fe645f?crop=entropy&cs=tinysrgb&fm=jpg&ixlib=rb-1.2.1&q=60&raw_url=true&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fGZyZWV8ZW58MHx8MHx8&auto=format&fit=crop&w=500',
            title: 'Blog Title 4',
            date: 'Wednesday May 25, 2022',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ornare pretium placerat ut platea...',
            linktext: 'Read article'
          }
        ]
      }
    }
  }
</script>