<template>
  <div>
    <client-only>
      <HeaderComponent />
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

export default {
  components: {
    HeaderComponent,
    FooterComponent
  }
}
</script>