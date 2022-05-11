<template>
  <client-only>
    <button v-show="scrollY > 300" id="backTop" class="btn-backtop" @click="toTop">
      <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-chevron-up" viewBox="0 0 16 16">
        <path fill-rule="evenodd" d="M7.646 4.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1-.708.708L8 5.707l-5.646 5.647a.5.5 0 0 1-.708-.708l6-6z"/>
      </svg>
    </button>
  </client-only>
</template>

<script>

export default {
  name: 'BackTop',

  data() {
    return {
      scrollTimer: 0,
      scrollY: 0
    }
  },

  mounted() {
    window.addEventListener('scroll', this.handleBackTopScroll);
  },

  methods: {
    handleBackTopScroll() {
      if (this.scrollTimer) return;
      this.scrollTimer = setTimeout(() => {
        this.scrollY = window.scrollY;
        clearTimeout(this.scrollTimer);
        this.scrollTimer = 0;
      }, 100);
    },

    toTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
    }
  }
}

</script>
