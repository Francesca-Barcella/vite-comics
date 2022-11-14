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
    
            <div class="card col-2">
                <img :src="image" :alt="title"> <!-- ok -->
                <h3>{{ title }}</h3> <!-- ok -->
            </div>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;


</style>