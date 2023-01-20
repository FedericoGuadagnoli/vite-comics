<script>
export default {
    name: 'AppFooterTop'
}
</script>


<template>
    <div class="footer-top">
        <div class="container">
            <div class="row">
                <div class="col">
                    <div class="products">
                        <div class="dc-comics">
                            <h2>DC COMICS</h2>
                            <ul>
                                <li>
                                    <a href="#">Characters</a>
                                </li>
                                <li>
                                    <a href="#">Comics</a>
                                </li>
                                <li>
                                    <a href="#">Movies</a>
                                </li>
                                <li>
                                    <a href="#">TV</a>
                                </li>
                                <li>
                                    <a href="#">Games</a>
                                </li>
                                <li>
                                    <a href="#">Videos</a>
                                </li>
                                <li>
                                    <a href="#">News</a>
                                </li>
                            </ul>
                        </div>
                        <div class="shop">
                            <h2>SHOP</h2>
                            <ul>
                                <li>
                                    <a href="#">Shop DC</a>
                                </li>
                                <li>
                                    <a href="#">Shop DC Collectibles</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="dc">
                        <h2>DC</h2>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy(New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choises</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact Us</a>
                            </li>
                        </ul>
                    </div>
                    <div class="sites">
                        <h2>SITES</h2>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col">
                    <figure>
                        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
                    </figure>
                </div>
            </div>
        </div>

    </div>
</template>


<style scoped>
.footer-top {
    height: 80%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
    height: 100%;
}

.row .col {
    flex-basis: 50%;
    display: flex;
    font-size: 1.25rem;
    gap: 5rem;
    height: 100%;
    overflow: hidden;
}

.col figure {
    width: 100%;
    text-align: end;
}

.col figure img {
    overflow: hidden;
}

ul li {
    margin: 10px 0;
    list-style-type: none;
}

.col h2 {
    margin: 50px 0 25px 0;
}

ul li a {
    color: white;
}
</style>