<script>

import AppNav from "/AppNav.vue"
// dobbiamo esportarlo per poterlo importare
export default {
    name:'AppHeader',
    components:{
        AppNav
    }

}
</script>

<template>
    <header class="top-box">Prova 123</header>
    <AppNav></AppNav>
</template>

<style scoped>
header{
    color: red;
}
</style>
