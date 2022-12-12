<script>

export default {
    name: "AppMain",
    }

</script>

<template>
    <main>

        <div class="container content">
            <div class="box">
                <h1> --> Content goes here!!! </h1>
            </div>
        </div>


        <div class="container service">

            <div class="box">

                <ul>
                    <li>
                        <img src="public/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </li>

                    <li>
                        <img src="public/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </li>

                    <li>
                        <img src="public/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </li>

                    <li>
                        <img src="public/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>

                    <li>
                        <img src="public/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>

            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


main {
    width: 100%;
    height: 300px;
    border: 1px solid black;
}

.container {
    width: 100%;
    height: 150px;
}
.box{
    max-width: 1400px;
    margin: 0 auto;
    height: 100%;
}

.content {
    background-color: $bg_secondary;
    color: $primary_color;
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

    li{
        display: flex;
        align-items: center;
        gap: 7px;
        font-size: 0.9rem;
    }

    img {
        width: 60px;
        height: 60px;
        object-fit:contain;
    }
}
</style>
