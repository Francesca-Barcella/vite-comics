<!-- Products per fabio -->

<script>
import ComicsList from '../data/dc-comics.js' /* ok */
import ComicsCard from '../components/MainComicsCard.vue'

export default {
    name: 'MainComicsCards', /* ok */
    components: {
        ComicsList,
        ComicsCard /* ok */
    },
    data() {
        return {
           cards: ComicsList /* ok */
                
        }
    }

}
</script>

<template>


   <div class="container py-5">
            <div class="cards row">
                <ComicsCard  v-for="item in cards" :image="item.thumb" :title="item.series"/> <!-- c'era una c minuscola invece di maiuscola!! cribbio -->
                <!-- <div class="card col-2" v-for="item in cards"> --ok con cards--
                    <img :src="item.thumb" --ok con thumb--
                        alt="">
                    <h3>{{item.series}}</h3> - ok con series--
                </div> -->
            </div>
        </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;
.cards {
        justify-content: space-between;
        flex-wrap: wrap;

  
    }
</style>