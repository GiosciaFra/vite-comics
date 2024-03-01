<script>
export default {
    name: 'AppLinks',
    data() {
        return {
            icons: [
                {
                    img: '/img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    img: '/img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    img: '/img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    img: '/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    img: '/img/buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },
            ]
        }
    },
}

</script>

<template>
    <div class="iconLinks">
        <div class="container">
            <div class="row">
                <div v-for="icon in icons" class="col">
                    <img :src="'/img/' + icon.img" :alt="icon.text">
                    <span>{{ icon.text }}</span>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/variables' as *;

.iconsLinks {
    background-color: $blueColor;

    .row {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 70px;
        padding: 50px;

        .col {
            display: flex;
            align-items: center;
            gap: 20px;
            height: 55px;

            img {
                max-width: 55px;
                height: 100%;
            }
        }
    }
}
</style>