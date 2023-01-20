<script>
export default {
    name: 'AppActions',
    data() {
        return {
            cards: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'subscriptions'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'comics shop locator'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'dc power visa'
                },

            ]


        }
    },

    methods: {
        buildImagePath(image) {
            const url = new URL(`../assets/img/${image}`,
                import.meta.url);
            return url.href;
        }
    }
}
</script>



<template>
    <ul>
        <li v-for="card in cards">
            <img :src="buildImagePath(card.image)" :alt="card.text">
            <a href="#">{{ card.text }}</a>
        </li>
    </ul>
</template>


<style lang="scss" scoped>
@use '../assets/scss/mixins' as *;

ul {
    @include center('between');
    height: 100%;

    li {
        list-style-type: none;
        @include center('center');
        gap: 1.25rem;
        flex-basis: calc(25% - 1.25rem);
        height: 60%;
        cursor: pointer;

        img {
            width: 5rem;
            height: auto;

        }

        a {
            color: white;
            font-size: x-large
        }
    }
}
</style>