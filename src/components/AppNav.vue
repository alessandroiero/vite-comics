<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name:'AppNav'
}
</script>

<template>
    <nav>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@use './styles/variables.scss' as *;
@use './styles/general.scss' as *;

    nav{
        ul{
            margin: 0;
            list-style: none;
        }
        li{
            a{
                display: inline-block;
                padding: 18px;
            }
        }
    }
</style>
