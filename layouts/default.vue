<template>
  <div id="app">
    <HeaderWeb />

    <Nuxt />

    <FooterWeb />
  </div>
</template>

<script>
import HeaderWeb from '@/components/HeaderWeb.vue'
import FooterWeb from '@/components/FooterWeb.vue'

export default {
  components: {
    HeaderWeb,
    FooterWeb,
  },
}
</script>
