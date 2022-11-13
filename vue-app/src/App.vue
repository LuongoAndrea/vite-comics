<template>
  <HeaderComponent/>
  <main>
    <ProductComponent/>
  </main>
  <FooterComponent/>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import ProductComponent from './components/ProductComponent.vue';

export default {
    components:{
        HeaderComponent,
        ProductComponent,
        FooterComponent,
        
    }
}

</script>

<style scoped>

</style>
