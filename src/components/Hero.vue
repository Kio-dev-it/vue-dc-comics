<template>
    <div class="hero" :style="`background-image: url(${bgImg})`">

    </div>
</template>

<script>
export default {
    name: 'Hero',
    props: ['bgImg']

}
</script>

<style lang="scss" scoped>
    
    .hero{
        height: 25rem;
        background-position: top;
        background-size: cover;
    }   

</style>