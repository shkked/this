<template>
  <div>
    <headerVue/>
    <div class="container">
      <nuxt class="nuxt"/>
    </div>
    <footerVue/>
  </div>
</template>

<script>
import footerVue from '../components/footer.vue'
import headerVue from '@/components/header.vue';
export default {
  components: {
    headerVue, footerVue
  },
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>

<style scoped>
  .nuxt{
      min-height: calc(100vh - 80px) !important;
  }
</style>
