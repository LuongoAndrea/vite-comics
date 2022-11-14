<template>
    <section>
        <JumboComponent/>
        <CardsComponent/>
    </section>
</template>

<script>
    import JumboComponent from './JumboComponent.vue';
    import CardsComponent from './CardsComponent.vue';
    export default {
        name:'ProductComponent.vue',
        components:{
            CardsComponent,
            JumboComponent
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    section{
        background-color: $black;
    }
</style>
