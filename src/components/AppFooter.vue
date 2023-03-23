<script>

import AppSocial from './AppSocial.vue';

export default {
    components: {
        AppSocial
    }
}
</script>

<template>
    <section class="cards">
        <div></div>
        <div>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <h3>DIGITAL COMICS</h3>
        </div>
        <div>
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <h3>DC MERCHANDISE</h3>
        </div>
        <div>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <h3>SUBSCRIPTION</h3>
        </div>
        <div>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <h3>COMIC SHOP LOCATOR</h3>
        </div>
        <div>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <h3>DC POWER VISA</h3>
        </div>
    </section>
    <section class="pre-footer">
        <div class="container pre-footer-content">
            <div class="social-links">
                <div>
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                        <li>Terms of use</li>
                        <li>Privacy policy</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div>
                    <h3>SITES</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <img class="logo-bg" src="../assets/img/dc-logo-bg.png" alt="DC logo">
        </div>
    </section>
    <section class="footer">
        <div class="container footer-content">
            <button class="sign-up">SIGN-UP NOW!</button>
            <AppSocial></AppSocial>
        </div>

    </section>
</template>

<style scoped>
.container {
    width: 80%;
    margin: 0 auto;
}


h3 {
    color: white;
}

li {
    color: #949495;
    list-style: none;
}

.cards {
    background-color: #0282f9;
    height: 155px;
    display: flex;
    gap: 60px;
    justify-content: center;
}

.cards div img {
    height: 35%;
}

.cards div h3 {
    color: white;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    font-size: 20px;
    font-weight: 100;
}

.cards div {
    display: flex;
    align-items: center;
    gap: 20px;
}

.pre-footer {
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    padding: 50px 0;
    overflow: hidden;
    height: 500px;
}

.pre-footer-content {
    display: flex;
    justify-content: space-between;
    height: 100%;
}

.social-links {
    display: flex;
    gap: 30px;
}

.social-links div ul {
    line-height: 35px;
    margin-top: 20px;
}

.logo-bg {
    height: 650px;
    position: relative;
    bottom: 100px
}

.footer {
    display: flex;
    background-color: #313130;
    padding: 30px 0;
}

.footer-content {
    display: flex;
    justify-content: space-between;
}

.sign-up {
    background-color: transparent;
    border: #0282f9 2px solid;
    padding: 10px;
    color: white;
}
</style>