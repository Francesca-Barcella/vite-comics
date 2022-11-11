<script>
export default {
    name: 'SiteHeader'
}
</script>

<template>
    <header id="site-header">
        <div class="container d-flex p-2">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="menu">
                <a href="#">link 1</a>
                <a href="#">link 2</a>
                <a href="#">link 3</a>
                <a href="#">link 4</a>
                <a href="#">link 5</a>
                <a href="#">link 6</a>
                <a href="#">link 7</a>
                <a href="#">link 8</a>
                <a href="#">link 9</a>
                <a href="#">link 10</a>
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

