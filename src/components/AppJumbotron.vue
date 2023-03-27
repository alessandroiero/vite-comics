<script>
export default {
    name: 'AppImg',
}
</script>

<template>
    <div class="img-full">
        <div class="main-bottom">
            <section class="container ">
            </section>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.img-full {
    background-image: url(../assets/img/jumbotron.jpg);
    width: 100%;
    height: 40vh;
}

.background-color {
    background-color: #1c1c1c;
}

h1 {

    color: white;
    padding: 30px;
}

.main-bottom {
    .container {
        display: flex;
        justify-content: space-between;
        padding: 30px 0 30px;
    }
}
</style>