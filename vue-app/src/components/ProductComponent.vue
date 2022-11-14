<template>
    <section class="container">

        <CardsComponent/>
    </section>
</template>

<script>
    import CardsComponent from './CardsComponent.vue';

    export default {
        name:'ProductComponent.vue',
        components:{
            CardsComponent
        }
    }
</script>

<style lang="scss" scoped>

</style>
