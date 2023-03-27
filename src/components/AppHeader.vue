<script>

import AppNav from "./AppNav.vue"
// dobbiamo esportarlo per poterlo importare
export default {
    name: 'AppHeader',
    components: {
        AppNav
    }

}
</script>

<template>
    <header>
        <div class="container">
            <div class="col-left">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="col-center"></div>
            <div class="col-right">
                <AppNav></AppNav>
            </div>
        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../assets/partials/variables' as *;
header {
    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        align-items:center;
        padding: 10px;
        
    }

    .col-left{
        flex-grow: 1;
    }

    background-color: $fourth_color;

}
</style>
