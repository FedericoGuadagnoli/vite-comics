<script>
export default {
    name: 'AppButton'
}
</script>


<template>
    <div>
        <button>load more</button>
    </div>

</template>


<style lang="scss" scoped>
@use '../assets/scss/mixins' as *;

div {
    @include center('center');
    padding: 2rem 0;

    button {
        text-transform: uppercase;
        color: white;
        padding: .8rem 3rem;
        font-size: 1.25rem;
        background-color: dodgerblue;
        cursor: pointer;
    }
}
</style>