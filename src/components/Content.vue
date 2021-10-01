<template>
    <main>
        <div class="container">
            <h2>Content goes here</h2>
        </div>
    </main>
</template>

<script>
export default {
    name: 'Content'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

main{
    background-color: #000;
    height: 120px; /*provisional*/
    
    h2{
        color: #fff;
        font-weight: 700;
    }
}

</style>