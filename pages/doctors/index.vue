<template>
	<client-only>
    <section class="ourdoctors">
      <div class="container p-0">
        <div class="ourdoctors-content">
          <div class="ourdoctors-header">
            
          </div>
          <div class="ourdoctors-body">
            <div class="row">
              <div class="col-lg-3 d-none d-lg-block">
                <FilterSidebar/>
              </div>
              
              <div class="col-lg-9 col-12">
                <AllDoc/>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
	</client-only>
</template>

<script>
  import FilterSidebar from '~/components/Filter/FilterSidebar/FilterSidebar';
  import AllDoc from '~/components/AllDoc/AllDoc';

  export default {
    name: 'DoctorsPage',
    components: {
      FilterSidebar,
      AllDoc,
    },
    data() {
      return {
        categories: [
          {title: 'ইউরোলোজি বিশেষজ্ঞ'},
          {title: 'ক্যান্সার ও টিউমার বিশেষজ্ঞ'},
          {title: 'গাইনী ও প্রসূতি বিশেষজ্ঞ'},
          {title: 'গাইনী সার্জন'},
          {title: 'গ্যাস্ট্রোলিভার বিষেশজ্ঞ'},
          {title: 'চর্ম ও যৌন রোগ বিশেষজ্ঞ'},
          {title: 'ডায়াবেটিস বিশেষজ্ঞ'},
          {title: 'নাক-কান-গলা রোগ বিশেষজ্ঞ'},
          {title: 'নিউরোমেডিসিন বিশেষজ্ঞ'},
          {title: 'ফিজিওথেরাপিষ্ট'},
          {title: 'বক্ষব্যাধি ও হৃদরোগ বিশেষজ্ঞ'},
          {title: 'বিশেষজ্ঞ পুষ্টিবিদ'},
          {title: 'বিশেষজ্ঞ সার্জন'},
          {title: 'মাথা ও মনোরোগ বিশেষজ্ঞ'},
          {title: 'মেডিসিন বিশেষজ্ঞ'},
          {title: 'ল্যাপারোস্কোপিক সার্জন'},
          {title: 'শিশুরোগ বিশেষজ্ঞ'},
          {title: 'হাড়-ভাঙ্গা বিশেষজ্ঞ'},
          {title: 'হেড-নেক সার্জন'},
        ]
      }
    },
  }
</script>
