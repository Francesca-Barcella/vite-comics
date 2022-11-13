<script>
import comics from '../data/dc-comics'

export default {
    name: 'Card'
}
</script>

<template>


   <div class="container py-5">
            <div class="cards row">
                <div class="card col-2" v-for="item in ComicsCards">
                    <img :src="item.thumb"
                        alt="">
                    <h3>{{item.series}}</h3>
                </div>
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