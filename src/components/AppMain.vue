<script>
import ListComics from './ListComics.vue';
export default {
    name: "AppMain",
    components: {
        ListComics
    },
}

</script>

<template>

        <div class="content">
            <div class="box">

                <h1 class="tag">CURRENT SERIES</h1>
                
                    <ListComics />

                <a class="tag" href="">LOAD MORE</a>

            </div>
        </div>


        <div class="container service">

            <div class="box">

                <ul>
                    <li>
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </li>

                    <li>
                        <img src="/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </li>

                    <li>
                        <img src="/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </li>

                    <li>
                        <img src="/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>

                    <li>
                        <img src="/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>

            </div>
        </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


main {
    width: 100%;
    border: 1px solid black;
}

.container {
    width: 100%;
    height: 150px;
}

.box {
    max-width: 1400px;
    margin: 0 auto;
    height: 100%;
    position: relative;
    text-align: center;

    h1 {
        width: 270px;
        position: absolute;
        top: -20px;
        padding: 15px 0;
    }

    a {
        padding: 10px 50px;
        color: white;
        text-decoration: none;
        display: inline-block;
        margin-bottom: 50px;
    }

    .tag {
        font-weight: 600;
        background-color: $bg_primary;
       
    }
}



.content {
    background-color: $bg_secondary;
    color: $primary_color;
    width: 100%;
}

.service {
    background-color: $bg_primary ;

    ul {
        display: flex;
        height: 100%;
        justify-content: space-around;
        align-items: center;
        color: $primary_color;

    }

    li {
        display: flex;
        align-items: center;
        gap: 7px;
        font-size: 0.9rem;
    }

    img {
        width: 60px;
        height: 60px;
        object-fit: contain;
    }
}
</style>
