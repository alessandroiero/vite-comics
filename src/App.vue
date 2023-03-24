<script>
// import HelloWorld from './components/HelloWorld.vue'
// importiamo i componenti
import AppHeader from "./components/AppHeader.vue"
import AppJumbotron from "./components/AppJumbotron.vue"
import AppMain from "./components/AppMain.vue"
import AppFooterList from "./components/AppFooterList.vue"
import AppFooter from "./components/AppFooter.vue"


// li esportiamo
export default {
  components:{
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFooterList,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppJumbotron></AppJumbotron>
  <AppMain></AppMain>
  <AppFooterList></AppFooterList>
  <AppFooter></AppFooter>
</template>

<!-- installo scss e non inserisco scoped -->
<style lang="scss">
// importiamo i file scss
@use './styles/variables.scss' as *;
@use './styles/general.scss' as *;

</style>
