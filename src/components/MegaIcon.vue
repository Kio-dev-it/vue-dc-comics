<template>
    <div class="mega-icon">
        <div class="mega-icon__logo">
            <img :src="iconInfo.src">
        </div>
        <div class="mega icon__text">
            {{iconInfo.title}}
        </div>
    </div>
</template>

<script>
export default {
    name: "MegaIcon",
    props: ['iconInfo']

}
</script>

<style lang="scss" scoped>
.mega-icon{
    display: flex;
    align-items: center;
    justify-content: space-between;
    
    &__logo{
        width: 3.125rem;
        height: 3.4375rem;
        margin-right: .5rem;

        img{
            object-fit: contain;
            height: 100%;
            width: 100%;
        }
    }
}

</style>