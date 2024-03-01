<script>
export default {
    name: 'AppComics',

    props: {
        name: String,
        image: String,
    }
}
</script>

<template>
    <div class="comic">
        <div class="comic-image">
            <img :src="image" alt="name">
        </div>
        <h3>{{ name }}</h3>
    </div>
</template>

<style lang="scss">
.comic {
    display: flex;
    flex-flow: column;
    align-items: center;
    width: calc(100% / 6 - 27px / 6 * 5);
    gap: 20px;

    .comic-image {
        width: 185px;
        height: 185px;
        overflow: hidden;

        img {
            width: 100%;
        }
    }
}
</style>