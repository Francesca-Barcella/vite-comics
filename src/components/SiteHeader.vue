<script>
export default {
    name: 'SiteHeader',
    data (){
        return {
            menu: [
                {
                    text:'characters',
                    href:'#'
                },
                {
                    text:'comics',
                    href:'#'
                },
                {
                    text:'movies',
                    href:'#'
                },
                {
                    text:'tv',
                    href:'#'
                },
                {
                    text:'games',
                    href:'#'
                },

                {
                    text:'collectibles',
                    href:'#'
                },
                {
                    text:'videos',
                    href:'#'
                },
                {
                    text:'fans',
                    href:'#'
                },
                {
                    text:'news',
                    href:'#'
                },
                {
                    text:'shop',
                    href:'#'
                }
            ]

        }
    }
}
</script>

<template>
    <header id="site-header">
        <div class="container d-flex py-2">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="menu">
                <a href="#" v-for="item in menu">{{item.text}}</a>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

header {
    background-color: $dc_ligth;

    .container {
        justify-content: space-between;
        align-items: center;
    }

    img {
        max-width: 70px;
    }

    a {
        color: $dc_dark;
        font-weight: 600;
        text-decoration: none;
        text-transform: uppercase;
        margin-left: 1rem;
        display: inline-block;
        border-bottom: 4px solid $dc_ligth;
        padding-bottom: 1rem;

        &:hover {
            color: $dc_primary;
            border-bottom: 4px solid $dc_primary;
            padding-bottom: 1rem;
        }
    }
}
</style>

