<script>
// import HelloWorld from './components/HelloWorld.vue'
// importiamo i componenti
import AppHeader from "./components/AppHeader.vue"
import AppJumbotron from "./components/AppJumbotron.vue"
import AppDescription from "./components/AppDescription.vue"
import AppFooterList from "./components/AppFooterList.vue"
import AppFooter from "./components/AppFooter.vue"
import AppCards from "./components/AppCards.vue"

// li esportiamo
export default {
  components:{
    AppHeader,
    AppJumbotron,
    AppDescription,
    AppCards,
    AppFooterList,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppJumbotron></AppJumbotron>
  <AppCards></AppCards>
  <AppDescription></AppDescription>
  <AppFooterList></AppFooterList>
  <AppFooter></AppFooter>
</template>

<!-- installo scss e non inserisco scoped -->
<style lang="scss">
// importiamo i file scss
@use 'assets/partials/variables' as *;
@use "assets/main.scss" as *;


</style>
