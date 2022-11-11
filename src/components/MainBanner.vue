<script>
export default {
    name: 'MainBanner',
    data() {
        return {
            items: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'comics shop locator'
                },
                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ]

        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <div class="main_banner">
        <div class="container">
            <div class="row d.flex py-2 px-5">
                <div class="col d-flex align-items-center" v-for="item in items">
                    <img :src="getImageUrl(item.img)" alt="">
                    <h5 class="ms-2">{{ item.text }}</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

.main_banner {
    background-color: #0282F9;

    .row {
        justify-content: space-evenly;
        text-align: center;

        img {
            width: 40px;
        }

        h5 {
            text-transform: uppercase;
        }
    }
}
</style>