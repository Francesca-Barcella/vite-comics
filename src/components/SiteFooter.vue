<script>
import FooterMenu from './FooterMenu.vue'

export default {
    name: 'SiteFooter',

    components: {
        FooterMenu,
    },

    data(){
        return{
            social:[
                {
                    url:'footer-facebook.png',
                },
                {
                    url:'footer-periscope.png',
                },
                {
                    url:'footer-pinterest.png',
                },
                {
                    url:'footer-twitter.png',
                },
                {
                    url:'footer-youtube.png',
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
    <footer id="site-footer">
        <FooterMenu />
        
        <div class="footer_bottom py-4">
            <div class="container bottom d-flex">
                <div class="cta p-2">
                    <a href="#" class="btn">SIGN-UP NOW!</a>
                </div>
                <div class="social d-flex">
                    <p>Follow us</p>
                    <div v-for="item in social">
                        <img :src="getImageUrl(item.url)" alt="">
                    </div>
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
            justify-content: space-bet;
            align-items: center;
            text-transform: uppercase;
        }
        p:hover{
            cursor: pointer;
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

