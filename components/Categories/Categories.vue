<template>
  <aside class="categorysidebar">
    <div class="categorysidebar-body">
      <ul class="sidebarlist">
        <li v-for="(category, i) in categories" :key="i" class="sidebarlist-item">
          <CategorySidebar :ctg-info=category />
        </li>
      </ul>
    </div>
  </aside>
</template>

<script>
  import CategorySidebar from '~/components/CategorySidebar/CategorySidebar';
  export default {
    name: 'Categories',
    components: {
      CategorySidebar
    },
    data() {
      return {
        categories: [
          {title: 'ইউরোলোজি বিশেষজ্ঞ', counter: 2},
          {title: 'ক্যান্সার ও টিউমার বিশেষজ্ঞ', counter: 3},
          {title: 'গাইনী ও প্রসূতি বিশেষজ্ঞ', counter: 6},
          {title: 'গাইনী সার্জন', counter: 5},
          {title: 'গ্যাস্ট্রোলিভার বিষেশজ্ঞ', counter: 5},
          {title: 'চর্ম ও যৌন রোগ বিশেষজ্ঞ', counter: 6},
          {title: 'ডায়াবেটিস বিশেষজ্ঞ', counter: 7},
          {title: 'নাক-কান-গলা রোগ বিশেষজ্ঞ', counter: 7},
          {title: 'নিউরোমেডিসিন বিশেষজ্ঞ', counter: 4},
          {title: 'ফিজিওথেরাপিষ্ট', counter: 1},
          {title: 'বক্ষব্যাধি ও হৃদরোগ বিশেষজ্ঞ', counter: 7},
          {title: 'বিশেষজ্ঞ পুষ্টিবিদ', counter: 1},
          {title: 'বিশেষজ্ঞ সার্জন', counter: 10},
          {title: 'মাথা ও মনোরোগ বিশেষজ্ঞ', counter: 1},
          {title: 'মেডিসিন বিশেষজ্ঞ', counter: 21},
          {title: 'ল্যাপারোস্কোপিক সার্জন', counter: 1},
          {title: 'শিশুরোগ বিশেষজ্ঞ', counter: 3},
          {title: 'হাড়-ভাঙ্গা বিশেষজ্ঞ', counter: 4},
          {title: 'হেড-নেক সার্জন', counter: 5}
        ]
      }
    }
  }
</script>