<script>

export default {
    name: 'AppNav',

    data() {
        return {
            links: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop"
            ],

            activeLinkIndex: 1,
        }
    }
}

</script>

<template>
    <nav>
        <img class="logo" src="/img/dc-logo.png" alt="">
        <ul class="links">
            <li v-for="(currentLink, index) in links" :class="index == activeLinkIndex ? 'active' : ''">
                {{ currentLink }}
            </li>
        </ul>
    </nav>
</template>

<style lang ="scss">
@use '../styles/variables.scss' as *;

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;

    height: 120px;

    padding: 0 200px;

    ul {
        display: flex;
        gap: 30px;

        li {
            list-style-type: none;
            text-transform: uppercase;
            font-size: 14px;
            font-weight: 600;

            &.active {
                color: $blueColor;

            }

        }
    }
}
</style>