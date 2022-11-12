<script>
import FooterMenu from './FooterMenu.vue'

export default {
    name: 'SiteFooter',
    components: {
        FooterMenu,
    }
}
</script>

<template>
    <footer id="site-footer">
        <FooterMenu />
        
        <div class="footer_bottom py-4">
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

    .footer_bottom {
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

        .social {
            justify-content: space-evenly;
            align-items: center;
            text-transform: uppercase;
        }

        img {
            padding-left: 1rem;

            &:hover {
                cursor: pointer;
            }
        }
    }

}
</style>

