<script>
export default {
    name: 'AppShop',
    data() {
        return {
            icons: [
                {
                    image: 'buy-comics-digital-comics.png',
                    title: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    title: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    title: 'subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    title: 'comic shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    title: 'dc power visa'
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
                    <img :src="'/img/' + icon.image" :alt="icon.title">
                    <span>{{ icon.title }}</span>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/variables' as *;

.iconLinks {
    background-color: $blueColor;
    color: white;
    text-transform: uppercase;

    .row {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 40px;
        padding: 50px;


        .col {
            display: flex;
            align-items: center;
            gap: 20px;
            height: 55px;
            white-space: nowrap;

            img {
                max-width: 55px;
                height: 100%;
            }
        }
    }
}
</style>