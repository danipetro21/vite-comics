<script>

export default {
    name: "JumboTron",
}

</script>

<template>


    <!-- card -->
    <section class="jumbo">

        <img src="/img/jumbotron.jpg" alt="">

    </section>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.jumbo{
    width: 100%;
    height: 500px;
    img{
        width: 100%;
        height: 100%;
        object-fit:cover;
        object-position: 0% 0%;
    }
}
</style>
