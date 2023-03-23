<script>
export default {
    data() {
        return {
            social: [
                {
                    name: 'facebook',
                    logo: 'src/assets/img/footer-facebook.png',
                    link: '#',
                    target: '_self',
                }, {
                    name: 'twitter',
                    logo: 'src/assets/img/footer-twitter.png',
                    link: '#',
                    target: '_self',
                }, {
                    name: 'youtube',
                    logo: 'src/assets/img/footer-youtube.png',
                    link: '#',
                    target: '_self',
                }, {
                    name: 'pinterest',
                    logo: 'src/assets/img/footer-pinterest.png',
                    link: '#',
                    target: '_self',
                }, {
                    name: 'periscope',
                    logo: 'src/assets/img/footer-periscope.png',
                    link: '#',
                    target: '_self',
                },
            ],
        }
    }
}
</script>

<template>
    <div>
        <h3>FOLLOW US</h3>
        <ul>
            <li v-for="item in social"><a :href="item.link"><img :src="item.logo"></a></li>
        </ul>
    </div>
</template>

<style scoped>
div {
    display: flex;
    align-items: center;
}

div h3 {
    padding: 0 16px;
    font-size: 20px;
    font-weight: bold;
    color: #0382f8;
}

div ul {
    display: flex;
    list-style-type: none;
    gap: 10px;
}

div ul li a {
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    width: 50px;
    height: 50px;
}

div ul li a img {
    max-width: 100%;
    object-fit: center;
}
</style>