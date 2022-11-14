<script>
import MainBanner from './MainBanner.vue'
import MainComicsCards from './MainComicsCards.vue' /* ok */

export default {
    name: 'SiteMain',
    components: {
        MainComicsCards,  /* ok */
        MainBanner
    }

}
</script>

<template>
    <main id="site-main">
        <MainComicsCards /> <!-- Products per fabio -->
        <!-- <div class="container py-5">
            <div class="cards row">
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                        alt="">
                    <h3>Action Comics</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01"
                        alt="">
                    <h3>American Vampire 1976</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb"
                        alt="">
                    <h3>Aquaman</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                        alt="">
                    <h3>Action Comics</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01"
                        alt="">
                    <h3>American Vampire 1976</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb"
                        alt="">
                    <h3>Aquaman</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                        alt="">
                    <h3>Action Comics</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01"
                        alt="">
                    <h3>American Vampire 1976</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb"
                        alt="">
                    <h3>Aquaman</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                        alt="">
                    <h3>Action Comics</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01"
                        alt="">
                    <h3>American Vampire 1976</h3>
                </div>
                <div class="card col-2">
                    <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb"
                        alt="">
                    <h3>Aquaman</h3>
                </div>
            </div>
        </div> -->
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

