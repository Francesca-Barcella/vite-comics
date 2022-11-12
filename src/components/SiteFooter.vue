<script>
export default {
    name: 'SiteFooter'
}
</script>

<template>
    <footer id="site-footer">
        <div class="container top py-2">
            <div class="row d-flex">
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
                    <h3 class="shop">SHOP</h3>
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
            </div>
        </div>
        <div class="bottom py-4">
            <div class="container bottom d-flex">
                <div class="cta p-2">
                    <a href="#" class="btn">SIGN-UP NOW!</a>
                </div>
                <div class="social d-flex">
                    <p>Follow us</p>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
@use '../assets/scss/partials/_variables.scss' as *;

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;

    .container.top {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;

        .row {
            justify-content: flex-start;
            padding-top: 1rem;
            padding-bottom: 1rem;

            h4,
            .shop {
                padding-bottom: 0.75rem;
            }

            .shop {
                padding-top: 0.75rem;
            }

            li {
                color: $dc_secondary_ligth;
                text-decoration: none;
                list-style: none;

                &:hover {
                    color: $dc_ligth;
                    cursor: pointer;
                }
            }

        }

    }

    .bottom {
        background-color: $dc_dark;
    }

    .container.bottom {
        justify-content: space-between;

        .cta {
            border: 1px solid $dc_primary;

            a {
                color: $dc_ligth;
                text-decoration: none;
            }
        }
        
        .social{
            justify-content: space-evenly;
            align-items: center;
            text-transform: uppercase;
        }

        img{
            padding-left: 1rem;
            &:hover{
                cursor: pointer;
            }
        }
    }

}
</style>

