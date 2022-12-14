<script>

export default {
    name: "Comic",
    props: ["details"]
}

</script>

<template>


    <!-- card -->
    <div class="comic-card">
        <img :src="details.thumb" alt="">
        <h3>{{ details.series }}</h3>
    </div>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.comic-card {
    
    width: calc(100% / 6);
    padding: 0 20px;

    h3 {
        margin: 10px 0;     
    }

    img {
        display: block;
        width: 100%;
        height: 200px;
        object-fit:cover;
    }
}
</style>
