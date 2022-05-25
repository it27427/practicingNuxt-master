<template>
  <!--========== BLOG-DESCRIPT START ==========-->
  <section class="blogdescript">
    <div class="container">
      <div v-for="(bigblog, i) in blogList" :key="i" class="card-blog">
        <BigBlog :blogs="bigblog" />
      </div>
    </div>
  </section>
  <!--========== BLOG-DESCRIPT END ============-->
</template>

<script>
  import BigBlog from '~/components/Cards/BigBlog';

  export default {
    name: 'BlogDescription',
    components: {
      BigBlog
    },
    data() {
      return {
        blogList: [
          {
            imageSrc: 'https://images.unsplash.com/photo-1538991383142-36c4edeaffde?crop=entropy&cs=tinysrgb&fm=jpg&ixlib=rb-1.2.1&q=60&raw_url=true&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NHx8ZnJlZXxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500',
            title: 'The hidden struggle of working moms? Guilt. How to overcome it',
            date: 'Wednesday May 25, 2022',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin lorem condimentum sed proin vitae eu. Consectetur diam mattis proin ut ut et Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consectetur diam mattis proin ut ut et Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
            linktext: 'Read More'
          }
        ]
      }
    }
  }
</script>