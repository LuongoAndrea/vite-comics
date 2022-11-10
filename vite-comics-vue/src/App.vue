<template>
  <HeaderComponent/>
  <main>
    <ListComponent/>
  </main>
  <FooterComponent/>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import ListComponent from './components/ListComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
export default {
  components:{HeaderComponent, ListComponent, FooterComponent}
}

</script>

<style scoped>

</style>
