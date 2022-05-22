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
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-one blog-regular",
          "author": "Istiak Hossain Tushar",
          "date": "Sunday, May 15, 2022"
        },
        {
          "id": "blog-2",
          "imgSrc": "https://images.unsplash.com/photo-1422255198496-21531f12a6e8?dpr=2&auto=format&fit=crop&w=1500&h=996&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-two blog-large",
          "author": "Abdullah Al Mamun",
          "date": "Saturday, May 14, 2022"
        },
        {
          "id": "blog-3",
          "imgSrc": "https://images.unsplash.com/photo-1490914327627-9fe8d52f4d90?dpr=2&auto=format&fit=crop&w=1500&h=2250&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-three blog-full",
          "author": "Rakibul Islam Rocky",
          "date": "Friday, May 13, 2022"
        },
        {
          "id": "blog-4",
          "imgSrc": "https://images.unsplash.com/photo-1476097297040-79e9e1603142?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-four blog-regular",
          "author": "Riazul Islam Hasan",
          "date": "Thursday, May 12, 2022"
        },
        {
          "id": "blog-5",
          "imgSrc": "https://images.unsplash.com/photo-1464652149449-f3b8538144aa?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-five blog-regular",
          "author": "Rajkumar Das",
          "date": "Wednesday, May 11, 2022"
        },
        {
          "id": "blog-6",
          "imgSrc": "https://images.unsplash.com/photo-1470124182917-cc6e71b22ecc?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-six blog-regular",
          "author": "Golam Foysal Nirjhor",
          "date": "Tuesday, May 10, 2022"
        },
        {
          "id": "blog-7",
          "imgSrc": "https://images.unsplash.com/photo-1422255198496-21531f12a6e8?dpr=2&auto=format&fit=crop&w=1500&h=996&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-seven blog-regular",
          "author": "Zesan Ul Banna",
          "date": "Monday, May 09, 2022"
        },
        {
          "id": "blog-8",
          "imgSrc": "https://images.unsplash.com/photo-1476097297040-79e9e1603142?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-eight blog-large",
          "author": "Rezaul Islam Reza",
          "date": "Sunday, May 08, 2022"
        },
        {
          "id": "blog-9",
          "imgSrc": "https://images.unsplash.com/photo-1464652149449-f3b8538144aa?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-nine blog-regular",
          "author": "Islam Sajal",
          "date": "Saturday, May 07, 2022"
        },
        {
          "id": "blog-10",
          "imgSrc": "https://images.unsplash.com/photo-1476097297040-79e9e1603142?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-eight blog-large",
          "author": "Milon Sarkar",
          "date": "Friday, May 06, 2022"
        },
        {
          "id": "blog-11",
          "imgSrc": "https://images.unsplash.com/photo-1464652149449-f3b8538144aa?dpr=2&auto=format&fit=crop&w=1500&h=1000&q=80&cs=tinysrgb&crop=",
          "title": "রমজানের সুস্থতা-Healthy Ramadan Fasting Tips-Doctortodays",
          "boxSize": "blog-nine blog-regular",
          "author": "Sadman Pratik",
          "date": "Thursday, May 05, 2022"
        }
      ]
    }
  }
}
</script>