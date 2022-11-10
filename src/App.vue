<script>
import SiteHeader from './components/SiteHeader.vue'
import SiteMain from './components/SiteMain.vue'

export default {
  name: 'Comics',
  components:{
    SiteHeader,
    SiteMain
  }
}
</script>

<template>
  <SiteHeader></SiteHeader>
  <SiteMain></SiteMain>

  <footer id="site-footer">
    footer
  </footer>

</template>

<style lang="scss">

</style>
