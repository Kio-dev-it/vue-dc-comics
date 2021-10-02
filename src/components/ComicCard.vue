<template>
    <div class="card">
        <div class="card__image">
            <div class="image-container">
                <img :src="comicInfo.thumb" :alt="comicInfo.series" class="comic-cover">
            </div>
        </div>
        <div class="card__title">
            <h3 class="comic-title">{{comicInfo.series}}</h3>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        comicInfo: Object
    }

}
</script>

<style lang="scss" scoped>
    .card{
        margin: 0 .9375rem 3.125rem .9375rem;

        width: calc( 100% / 6 - 30px );

        .card__image{
            margin-bottom: 1.25rem;

            .image-container{
                width: 100%;
                padding-bottom: 100%;
                position: relative;
            }
            img{
                width: 100%;
                height: 100%;
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0;
                object-fit: cover;
                object-position: top;
            }
        }

        .card__title{
            font-weight: 700;
            color: #fff;
            font-size: .6875rem;

            .comic-title{
                text-transform: uppercase;
            }
        }
    }


</style>