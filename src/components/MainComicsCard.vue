<script>
export default {
    name: 'MainComicsCard',
    props: { /* ok */
        image: String, /* ok */
        title: String /* ok */
    }
}
</script>

<template>
    <div class="container py-5">
        <div class="row cards">
            <div class="card col-2">
                <img :src="image" :alt="title"> <!-- ok -->
                <h3>{{ title }}</h3> <!-- ok -->
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;


</style>