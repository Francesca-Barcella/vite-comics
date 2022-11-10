<script>
export default {
    name: 'SiteMain'
}
</script>

<template>
    <main id="site-main">
        <div class="top">
            Content goes here
        </div>
        <div class="bottom">
            <div class="row">
                <div class="col">DIGITAL COMICS</div>
                <div class="col">DC MERCHANDISER</div>
                <div class="col">SUBSCRIPTION</div>
                <div class="col">COMIC SHOP LOCATOR</div>
                <div class="col">DC POWER VISA</div>
            </div>
        </div>
    </main>
</template>

<style lang="scss">
main {
    background-color: black;
    color: white;

    .top {
        height: 30vh;
        max-width: 80%;
        margin: auto;
        line-height: 30vh;
    }

    .bottom {
        background-color: #0282F9;
    }

    .row {
        display: flex;
        justify-content: space-between;
        max-width: 80%;
        margin: auto;
        border: 1px solid white;
        padding: 2rem;
    }

}
</style>

