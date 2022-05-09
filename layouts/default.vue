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
  </div>
</template>

<script>
import HeaderComponent from '~/components/HeaderComponent/HeaderComponent';
import FooterComponent from '~/components/FooterComponent/FooterComponent';
import Gap from '~/components/Gap/Gap';

export default {
  components: {
    HeaderComponent,
    FooterComponent,
    Gap
  }
}
</script>