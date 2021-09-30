<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/images/dc-logo.png" alt="DC Comics Logo">
            </div>
            <div class="menu">
                <ul>
                    <li v-for="(page, index) in pages" :key="index"><a :href="page.hRef" :class="{ active: page.currentPage}">{{page.pageName}}</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header', 
    data() {
        return {
            pages: [
                {
                    hRef: '#',
                    pageName: 'CHARACTERS',
                    currentPage: false
                },
                {
                    hRef: '#',
                    pageName: 'COMICS',
                    currentPage: true
                },
                {
                    hRef: '#',
                    pageName: 'MOVIES',
                    currentPage: false
                },
                                {
                    hRef: '#',
                    pageName: 'TV',
                    currentPage: false
                },
                {
                    hRef: '#',
                    pageName: 'GAMES',
                    currentPage: false
                },
                {
                    hRef: '#',
                    pageName: 'COLLECTIBLES',
                    currentPage: false
                },
                                {
                    hRef: '#',
                    pageName: 'VIDEOS',
                    currentPage: false
                },
                                {
                    hRef: '#',
                    pageName: 'FANS',
                    currentPage: false
                },
                {
                    hRef: '#',
                    pageName: 'NEWS',
                    currentPage: false
                },
                {
                    hRef: '#',
                    pageName: 'SHOP',
                    currentPage: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

header{
    background-color: #fff;
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        
        li {
            list-style: none;
            display: inline-block;
            padding: 0 .375rem;

            a{
                display: inline-block;
                height: 8.125rem;
                line-height: 8.125rem;
                text-decoration: none;
                color: #000;
                font-weight: 700;

                &.active{
                    border-bottom: 6px solid $mainColor;
                    color: $mainColor;
                }

            }
        }
    }
}

</style>