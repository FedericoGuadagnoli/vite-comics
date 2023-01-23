<script>
export default {
    name: 'AppMain',
    props: {
        cards: Array
    }
};
</script>


<template>
    <div class="main-info">
        <h2>CURRENT SERIES</h2>
    </div>
    <div class="row">
        <div class="card" v-for="card in cards" :key="card.series">
            <figure>
                <img :src="card.thumb" :alt="card.series">
            </figure>
            <figcaption>{{ card.series }}</figcaption>
        </div>
    </div>

</template>


<style scoped lang="scss">
.main-info {
    position: absolute;
    background-color: dodgerblue;
    padding: .5rem;
    bottom: 97%;
}

.row {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    gap: 2rem;
    padding: 3rem 1rem;

    .card {
        flex-basis: calc(100% / 6 - 2rem);
        height: 350px;

        figure {
            height: 80%;

            img {
                width: 100%;
                height: 100%;
                display: block;
            }
        }

        figcaption {
            margin-top: 1rem;
        }
    }
}
</style>