<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="footer-bottom__left">
                <a href="#" class="sign-up">SIGN UP NOW!</a>
            </div>

            <div class="footer-bottom__right">
                <a href="#" class="follow">FOLLOW US</a>
                <a v-for="(link, index) in Social" :key="index" :href="link.src"> <img :src="link.img" :alt="link.name"></a>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: "FooterBottom",
    data() {
        return{
            Social: [
                {
                    name: 'Facebook',
                    src: 'https://www.facebook.com/dc',
                    img: require('../assets/images/footer-facebook.png')
                },
                {
                    name: 'Twitter',
                    src: 'https://www.twitter.com',
                    img: require('../assets/images/footer-twitter.png')
                },
                {
                    name: 'Youtube',
                    src: 'https://www.youtube.com',
                    img: require('../assets/images/footer-youtube.png')
                },
                {
                    name: 'Pinterest',
                    src: 'https://www.pinterest.com',
                    img: require('../assets/images/footer-pinterest.png')
                },
                {
                    name: 'Periscope',
                    src: 'https://www.periscope.com',
                    img: require('../assets/images/footer-periscope.png')
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

.footer-bottom{
    background-color: #303030;
    padding: 2.1875rem 0;

    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;

        .sign-up{
            text-decoration: none;
            display: inline-block;
            border: .1875rem solid $mainColor;
            color: #fff;
            font-weight: 700;
            padding: .5rem;
        }

        .footer-bottom__right{
            display: flex;
            align-items: center;
        
            .follow{
                text-decoration: none;
                font-weight: 700;
                color: $mainColor;
                margin-right: 2.1875rem;
            }

            a{
                display: inline-block;

                &:not(:last-child){
                    margin-right: 1.25rem;
                }
            }
        }
    }
}
</style>