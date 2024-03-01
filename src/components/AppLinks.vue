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
        <div v-for="(actualIcon, index) in icons" class="icon">

        </div>
    </div>
</template>

<style></style>