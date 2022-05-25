<template>
	<client-only>
    <section class="contact">
      <ContactForm/>
    </section>
	</client-only>
</template>

<script>
  import ContactForm from '~/components/ContactForm/ContactForm'
  export default {
    name: 'ContactPage',
    components: {
      ContactForm
    }
  }
</script>