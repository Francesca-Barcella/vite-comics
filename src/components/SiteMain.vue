<script>
import MainBanner from './MainBanner.vue'

export default {
    name: 'SiteMain',
    components:{
        MainBanner,
    }

}
</script>

<template>
    <main id="site-main">
        <div class="container top py-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab cupiditate libero ullam et adipisci
            necessitatibus, nihil architecto illo non, rem facere. Praesentium, debitis et. Tempora sit et ipsa
            laudantium ut. Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab cupiditate libero ullam et
            adipisci necessitatibus, nihil architecto illo non, rem facere. Praesentium, debitis et. Tempora sit et ipsa
            laudantium ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab cupiditate libero ullam et
            adipisci necessitatibus, nihil architecto illo non, rem facere. Praesentium, debitis et. Tempora sit et ipsa
            laudantium ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab cupiditate libero ullam et
            adipisci necessitatibus, nihil architecto illo non, rem facere. Praesentium, debitis et. Tempora sit et ipsa
            laudantium ut.Tempora sit et ipsa laudantium ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab
            cupiditate libero ullam et adipisci necessitatibus, nihil architecto illo non, rem facere. Praesentium,
            debitis et. Tempora sit et ipsa laudantium ut.Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab
            cupiditate libero ullam et adipisci necessitatibus, nihil architecto illo non, rem facere. Praesentium,
            debitis et. Tempora sit et ipsa laudantium ut.
        </div>
        <!-- serve per richiamare il banner nell'altro components -->
        <MainBanner />

    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

main {
    background-color: $dc_dark;
    color: $dc_ligth;

}
</style>

