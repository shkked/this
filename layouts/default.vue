<template>
  <div>
    <headerVue/>
      <nuxt class="nuxt"/>
    <footerVue/>
  </div>
</template>

<script>
import footerVue from '@/components/common/footer.vue'
import headerVue from '@/components/common/header.vue';
export default {
  components: {
    headerVue, footerVue
  },
  name: 'DefaultLayout',
  data () {
    return {

    }
  }
}
</script>

<style scoped>
  .nuxt{
      min-height: calc(100vh - 80px) !important;
  }
</style>
