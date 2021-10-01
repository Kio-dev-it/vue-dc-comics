<template>
    <div class="mega-icons">
        <div class="container">
            <MegaIcon v-for="(elm, index) in MegaIconInfo" :key="index" :iconInfo="elm"/>
        </div>
    </div>
</template>

<script>
import MegaIcon from './MegaIcon.vue'

export default {
    name: 'MegaIcons',
    components: {
        MegaIcon
    },
    data() {
        return {
            MegaIconInfo: [
                {
                    src: require("../assets/images/buy-comics-digital-comics.png"),
                    title: 'DIGITAL COMICS'
                },
                {
                    src: require("../assets/images/buy-comics-merchandise.png"),
                    title: 'DC MERCHANDISE'
                },
                {
                    src: require("../assets/images/buy-comics-subscriptions.png"),
                    title: 'SUBSCRIPTION'
                },
                {
                    src: require("../assets/images/buy-comics-shop-locator.png"),
                    title: 'COMIC SHOP LOCATOR'
                },
                {
                    src: require("../assets/images/buy-dc-power-visa.svg"),
                    title: 'DC POWER VISA'
                }
            ]
        }
    }


}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

.mega-icons{
    color: #fff;
    background-color: $mainColor;
    
    .container{
        display: flex;
        justify-content: space-around;
        padding: 3.4375rem 0;
    }
}

</style>