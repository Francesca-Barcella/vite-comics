<script>
export default {
    name: 'FooterMenu',
    data() {
        return {
            comics: [
                {
                    text: 'Characters',
                },
                {
                    text: 'Comics',
                },
                {
                    text: 'Movies',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'Games',
                },
                {
                    text: 'Videos',
                },
                {
                    text: 'News',
                }
            ],

            shop: [
                {
                    text: 'Shop DC',
                },
                {
                    text: 'Shop DC Collectibles',
                }
            ],

            dc: [
                {
                    text: 'terms Of Use',
                },
                {
                    text: 'Privacy Policy (New)',
                },
                {
                    text: 'Ad Choices',
                },
                {
                    text: 'Advertising',
                },
                {
                    text: 'Jobs',
                },
                {
                    text: 'Subscriptions',
                },
                {
                    text: 'Talent Workshops',
                },
                {
                    text: 'CPCS Certificates',
                },
                {
                    text: 'Rating',
                },
                {
                    text: 'Shop Help',
                },
                {
                    text: 'Contact Us',
                }
            ],

            sites: [
                {
                    text: 'DC',
                },
                {
                    text: 'MAD magazine',
                },
                {
                    text: 'DC Kids',
                },
                {
                    text: 'DC Power Visa',
                }
            ]
        }
    }

}
</script>

<template>
    <div class="container top py-2">
        <div class="row d-flex">
            <div class="col-2">
                <h4>DC COMICS</h4>
                <ul v-for="item in comics">
                    <li>{{ item.text }}</li>
                </ul>
                <h4 class="shop">SHOP</h4>
                <ul v-for="item in shop">
                    <li>{{ item.text }}</li>
                </ul>
            </div>
            <div class="col-2">
                <h4>DC</h4>
                <ul v-for="item in dc">
                    <li>{{ item.text }}</li>
                </ul>
            </div>
            <div class="col-2">
                <h4>SITES</h4>
                <ul v-for="item in sites">
                    <li>{{ item.text }}</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

</style>