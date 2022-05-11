<template>
  <div>
    <client-only>
      <HeaderComponent />
    </client-only>

    <client-only>
      <Gap />
    </client-only>

    <nuxt/>

    <client-only>
      <FooterComponent />
    </client-only>

    <client-only>
      <BackTop />
    </client-only>
  </div>
</template>

<script>
import HeaderComponent from '~/components/HeaderComponent/HeaderComponent';
import FooterComponent from '~/components/FooterComponent/FooterComponent';
import Gap from '~/components/Gap/Gap';
import BackTop from '~/components/BackTop/BackTop';

export default {
  components: {
    HeaderComponent,
    FooterComponent,
    Gap,
    BackTop
  }
}
</script>