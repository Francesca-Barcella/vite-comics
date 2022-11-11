<script>
export default {
    name: 'SiteFooter'
}
</script>

<template>
    <footer id="site-footer">
        <div class="container_top">
            <div class="row">
                <div class="col-2">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li>link 1</li>
                        <li>link 2</li>
                        <li>link 3</li>
                        <li>link 4</li>
                        <li>link 5</li>
                        <li>link 6</li>
                        <li>link 7</li>
                    </ul>
                    <h4 class="shop">SHOP</h4>
                    <ul>
                        <li>link 1</li>
                        <li>link 2</li>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>DC</h4>
                    <ul>
                        <li>link 1</li>
                        <li>link 2</li>
                        <li>link 3</li>
                        <li>link 4</li>
                        <li>link 5</li>
                        <li>link 6</li>
                        <li>link 7</li>
                        <li>link 8</li>
                        <li>link 9</li>
                        <li>link 10</li>
                        <li>link 11</li>
                    </ul>
                </div>
                <div class="col-2">
                    <h4>SITES</h4>
                    <ul>
                        <li>link 1</li>
                        <li>link 2</li>
                        <li>link 3</li>
                        <li>link 4</li>
                        <li>link 5</li>
                    </ul>
                </div>
                <div class="col-6">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="container_bottom">
            <div class="row">
                <div class="col sx">
                    <button> SING-UP NOW!</button>
                </div>
                <div class="col dx">
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-pinterest"></i>
                    <i class="fa-solid fa-location-dot"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
footer {
    background-image: url('../assets/img/footer-bg.jpg');

    .container_top {
        border: 1px solid red;
        max-width: 80%;
        margin: auto;
        padding-top: 1rem;
        padding-bottom: 1rem;
    }

    .row {
        display: flex;
        justify-content: space-between;
    }

    .col-1 {
        width: calc(100% / 12 * 1);
    }

    .col-6 {
        width: calc(100% / 12 * 9);
    }

    h4 {
        color: white;
        padding-bottom: 0.75rem;
    }

    .shop {
        padding-top: 0.75rem;
    }

    li {
        color: #959595;
        text-decoration: none;
        list-style: none;

    }

    img {
        max-width: 200px;
    }

    .container_bottom {
        background-color: #797979;

        .row {
            max-width: 80%;
            margin: auto;
        }
    }

}
</style>

