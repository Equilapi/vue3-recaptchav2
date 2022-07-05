<script>
import { ref } from 'vue'
import { VueRecaptcha } from 'vue-recaptcha';

export default {
  setup() {
    const sitekey = ref(import.meta.env.VITE_RECAPTCHAV2_SITEKEY)
    return {
      sitekey
    }
  },
  components: {
    VueRecaptcha
  }
}


</script>

<template>
  <main>
    <!-- <TheWelcome /> -->
    <vue-recaptcha :sitekey="sitekey"></vue-recaptcha>
  </main>
</template>