<template>
  <aside class="filtersidebar">
    <div class="filteroption">
      <label for="category">Doctor</label>
      <select id="category" class="category-select">
        <option v-for="(category, i) in categories" :key="i">
          <CategoryOption :ctg-info=category />
        </option>
      </select>
    </div>

    <div class="filteroption">
      <label for="districts">Distirct</label>
      <select id="districts" class="category-select">
        <option v-for="(district, i) in districts" :key="i">
          <DistrictOption :dts-info=district />
        </option>
      </select>
    </div>

    <div class="filteroption">
      <label for="thana">Thana</label>
      <select id="thana" class="category-select">
        <option v-for="(thana, i) in thanas" :key="i">
          <ThanaOption :thana-info=thana />
        </option>
      </select>
    </div>
  </aside>
</template>

<script>
  import CategoryOption from '~/components/Filter/Options/CategoryOption';
  import DistrictOption from '~/components/Filter/Options/DistrictOption';
  import ThanaOption from '~/components/Filter/Options/ThanaOption';
  export default {
    name: 'FilterSidebar',
    components: {
      CategoryOption,
      DistrictOption,
      ThanaOption,
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
          {title: 'হেড-নেক সার্জন'}
        ],
        districts: [
          {name: 'Sherpur'},
          {name: 'Dhaka'},
          {name: 'Barishal'},
          {name: 'Sylhet'},
          {name: 'Khulna'},
          {name: 'Chittagong'},
          {name: 'Rangpur'},
          {name: 'Mymensingh'}
        ],
        thanas: [
          {name: 'Sherpur Sadar'},
          {name: 'Nakla'},
          {name: 'Nalitabari'},
          {name: 'Sribordi'},
          {name: 'Jhenaigati'},
          {name: 'Uttara'},
          {name: 'Khilkhet'},
        ]
      }
    }
  }
</script>