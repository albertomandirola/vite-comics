<script>
export default {
    data() {
        return {
            links: [
                {
                    name: 'DIGITAL COMICS',
                    img: '/src/assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    img: '/src/assets/img/buy-comics-merchandise.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    img: '/src/assets/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'SUBSCRIPTIONS',
                    img: '/src/assets/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'DC POWER-VISA',
                    img: '/src/assets/img/buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>
<template lang="">
<div class="bluebanner">
    <div class="container">
        <ul>
            <li v-for='link, index in links'>
                <img :src="link.img" alt="">
                {{link.name}}

            </li>
        </ul>
    </div>
</div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.bluebanner {
    background-color: $primary_color;
    width: 100vw;
}

ul {
    background-color: $primary_color;
    @include orizontal-list;
    width: 100%;

    li {
        @include vertical-center;
        justify-content: center;
        width: calc(100% / 5);
        color: white;

        img {
            width: 50px;
            padding: 100px 10px 100px 0px;

        }
    }
}
</style>