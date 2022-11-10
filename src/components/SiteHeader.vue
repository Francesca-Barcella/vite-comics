<script>
export default {
    name: 'SiteHeader'
}
</script>

<template>
    <header id="site-header">
        <div class="container">
            <div class="log">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav>
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
            </nav>
        </div>
    </header>
</template>

<style lang="scss">
header {
    background-color: white;
    
    .container {
        border: 1px solid red;
        max-width: 80%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 1rem;
        padding-bottom: 1rem;
    }

    img {
        max-width: 70px;
    }

    a {
        color: black;
        text-decoration: none;
        margin-left: 1rem;
        display: inline-block;
    }
}
</style>

