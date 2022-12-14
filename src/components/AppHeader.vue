<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                }

            ]
        }
    },
}

</script>

<template>

    <header>

        <div class="container">
            <a href="">
                <img src="public/img/dc-logo.png" alt="">

            </a>

            <nav>
                <ul>
                        <li :class="{link: link.current}" v-for="(link, index) in links" :key="index">
                            <a :href="link.url" :class="{ active: link.current }">
                                {{ link.text }}
                            </a>
                        </li>
                </ul>
            </nav>

        </div>
    </header>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


header {
    text-align: center;


}

.container {
    @include center();
    max-width: 1400px;
    height: 150px;

    margin: 0 auto;

    img {
        width: 100%;
    }

    .link {
        height: 150px;
        border-bottom: 6px $text_color solid;
        display: flex;
        align-items: center;
    }

}

ul {
    list-style: none;
    @include center();

    li a {
        padding: 15px;
        color: black;
        text-decoration: none;
        transition: background 0.3s;
        font-size: 0.9rem;
        
        &.active,
        &:hover {
            color: $text_color;
        }
    }
}
</style>
