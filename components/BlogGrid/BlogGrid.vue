<template>
  <div>
    <div class="blog-grid">
      <BlogCard v-for="(blog, i) in blogInfoList" :key="i" :blog-info=blog />
    </div>
  </div>
</template>

<script>
import BlogCard from '~/components/Cards/BlogCard';

export default {
  name: 'BlogGrid',

  components: {
    BlogCard
  },

  data() {
    return {
      blogInfoList: [
        {
          "id": "blog-1",
          "imgSrc": "https://images.unsplash.com/photo-1470124182917-cc6e71b22ecc?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "jelly-o brownie sweet",
          "boxSize": "blog-one blog-regular"
        },
        {
          "id": "blog-2",
          "imgSrc": "https://images.unsplash.com/photo-1422255198496-21531f12a6e8?dpr=2&auto=format&fit=crop&w=1500&h=996&q=80&cs=tinysrgb&crop=",
          "title": "Muffin jelly gingerbread",
          "boxSize": "blog-two blog-large"
        },
        {
          "id": "blog-3",
          "imgSrc": "https://images.unsplash.com/photo-1490914327627-9fe8d52f4d90?dpr=2&auto=format&fit=crop&w=1500&h=2250&q=80&cs=tinysrgb&crop=",
          "title": "sesame snaps chocolate",
          "boxSize": "blog-three blog-full"
        },
        {
          "id": "blog-4",
          "imgSrc": "https://images.unsplash.com/photo-1476097297040-79e9e1603142?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "Oat cake",
          "boxSize": "blog-four blog-regular"
        },
        {
          "id": "blog-5",
          "imgSrc": "https://images.unsplash.com/photo-1464652149449-f3b8538144aa?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "jujubes cheesecake",
          "boxSize": "blog-five blog-regular"
        },
        {
          "id": "blog-6",
          "imgSrc": "https://images.unsplash.com/photo-1470124182917-cc6e71b22ecc?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "Dragée pudding brownie",
          "boxSize": "blog-six blog-regular"
        },
        {
          "id": "blog-7",
          "imgSrc": "https://images.unsplash.com/photo-1422255198496-21531f12a6e8?dpr=2&auto=format&fit=crop&w=1500&h=996&q=80&cs=tinysrgb&crop=",
          "title": "powder toffee",
          "boxSize": "blog-seven blog-regular"
        },
        {
          "id": "blog-8",
          "imgSrc": "https://images.unsplash.com/photo-1476097297040-79e9e1603142?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "pudding cheesecake",
          "boxSize": "blog-eight blog-large"
        },
        {
          "id": "blog-9",
          "imgSrc": "https://images.unsplash.com/photo-1464652149449-f3b8538144aa?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "toffee bear claw",
          "boxSize": "blog-nine blog-regular"
        }
      ]
    }
  }
}
</script>