<template>
    <main>
        <div class="container">
            <div class="collection-type">
                CURRENT SERIES
            </div>
            <ComicCard v-for="(elm, index) in comicInfo" :key="index" :comicInfo="elm"/>
        </div>
        <a href="#" class="load">LOAD MORE</a>
    </main>
</template>

<script>
import ComicCard from './ComicCard.vue';
import comics from '../assets/data/dc-comics.json'

export default {
    name: 'Content',
    components: {
        ComicCard
    },
    data(){
        return {
            comicInfo: comics,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    main{
        background-color: #000;
        padding: 4.0625rem 0 1rem 0; 
        color: #fff;

        .container{
            display: flex;
            flex-wrap: wrap;
            position: relative;

            .collection-type{
                position: absolute;
                left: 0;
                top: -4.0625rem;
                transform: translateY(-50%);
                background-color: $mainColor;
                padding: .5rem 1rem;
                font-weight: 700;
                font-size: 1.5rem;
            }
        }

        .load{
            display: inline-block;
            text-decoration: none;
            padding: .5rem 1.5rem;
            background-color: $mainColor;
            position: relative;
            left: 50%;
            transform: translateX(-50%);
            font-weight: 700;
            color: #fff;
        }
        
    }

</style>