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
        <div class="container">
            <img class="logo" src="/img/dc-logo.png" alt="DC Logo">
            <ul class="links">
                <li v-for="(currentLink, index) in links" :class="index == activeLinkIndex ? 'active' : ''">
                    {{ currentLink }}
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang ="scss">
@use '../styles/variables.scss' as *;

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;

    height: 120px;

    font-family: 'Barlow Condensed', sans-serif;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        width: 100%;
    }

    .logo {
        height: 80px;
    }

    ul.links {
        display: flex;
        align-items: stretch;
        gap: 30px;
        align-items: stretch;
        list-style-type: none;
        text-transform: uppercase;
        font-weight: bold;
        margin: 0;

        li {
            position: relative;
            display: flex;
            align-items: center;


            &.active {
                color: $blueColor;
                position: relative;
            }

            &.active::before {
                content: '';
                position: absolute;
                width: 100%;
                height: 5px;
                background-color: $blueColor;
                top: 66px;
                left: 0;
            }

        }
    }
}
</style>