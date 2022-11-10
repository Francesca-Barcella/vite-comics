<script>
import SiteHeader from './components/SiteHeader.vue'
import SiteMain from './components/SiteMain.vue'
import SiteFooter from './components/SiteFooter.vue'


export default {
  name: 'Comics',
  components:{
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<template>
  <SiteHeader></SiteHeader>

  <SiteMain></SiteMain>

  <SiteFooter></SiteFooter>
</template>

<style lang="scss">

</style>
