<template>
    <div class="footer-top">
        <div class="container">

            <div class="footer-lists">

                <div class="list-card" id="dc-comics">
                    <div class="list-card__name">
                        DC COMICS
                    </div>

                    <ul class="list-card__list">
                        <li v-for="(elm, index) in DcComics" :key="index">{{elm}}</li>
                    </ul>
                </div>

                <div class="list-card" id="shop">
                    <div class="list-card__name">
                        SHOP
                    </div>

                    <ul class="list-card__list">
                        <li v-for="(elm, index) in Shop" :key="index">{{elm}}</li>
                    </ul>
                </div>

                <div class="list-card" id="dc">
                    <div class="list-card__name">
                        DC
                    </div>

                    <ul class="list-card__list">
                        <li v-for="(elm, index) in DC" :key="index">{{elm}}</li>
                    </ul>
                </div>

                <div class="list-card" id="sites">
                    <div class="list-card__name">
                        SITES
                    </div>

                    <ul class="list-card__list">
                        <li v-for="(elm, index) in Sites" :key="index">{{elm}}</li>
                    </ul>
                </div>

            </div>
            <div class="footer-logo">
                <img src="../assets/images/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterTop",
    data(){
        return {
            DcComics: [
                'Characters',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],
            DC: [
                'Term of Use',
                'Privacy policy (New)',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshop',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            Sites: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ],
            Shop: [
                'Shop DC',
                'Shop DC Collectibles'
            ]
        }
    }

}
</script>

<style lang="scss" scoped>

.footer-top{
    background-image: url('../assets/images/footer-bg.jpg');
    color: #959595;

    .container{
        display: flex;
        justify-content: space-between;
        height: 26rem;

    }

    .footer-lists{
        padding: 2.8125rem 0 3.75rem 0;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        width: 30.75rem;
    
        .list-card{
            margin-right: 1.875rem;

            &__name{
                color: #fff;
                font-weight: 700;
                font-size: 1.25rem;
                margin-bottom: 1.25rem;
            }

            &__list{
                list-style: none;
                margin-bottom: 1.25rem;

                li{
                    margin-bottom: .375rem;
                }
            }
        }
    }

    .footer-logo{
        width: 35rem;

        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }

}

</style>