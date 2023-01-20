<script>
export default {
    name: 'AppFooterBottom'
}
</script>


<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="row">
                <div class="col">
                    <button class="btn">sign-up now!</button>
                </div>
                <div class="col">
                    <span>follow us</span>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">

                </div>
            </div>
        </div>
    </div>

</template>


<style lang="scss" scoped>
@use '../assets/scss/mixins' as *;

.footer-bottom {
    background-color: #303030;
    height: 20%;

    .row {
        height: 100%;
        @include center('between');

        .col {
            @include center('');
            gap: 2rem;
            font-size: 1.25rem;
            text-transform: uppercase;
            color: rgb(16, 120, 224);

            .btn {
                background-color: transparent;
                font-size: 1.25rem;
                padding: 15px;
                border: 3px solid rgb(16, 120, 224);
                color: white;
                text-transform: uppercase;
            }

        }
    }
}
</style>