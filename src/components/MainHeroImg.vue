<script>
export default {
    name: 'MainHeroImg',
    }
</script>

<template>
   <div class="hero_img">
   </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;
.hero_img{
   background-image: url('../assets/img/jumbotron.jpg');
   background-size: cover;
   height: 400px;
}
</style>