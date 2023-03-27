<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name:'AppNav'
}
</script>

<template>
    <nav>
        <ul>
            <li><a href="">CHARACTERS</a></li>
            <li><a href="">COMICS</a></li>
            <li><a href="">MOVIES</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">GAMES</a></li>
            <li><a href="">COLLECTIBLES</a></li>
            <li><a href="">VIDEOS</a></li>
            <li><a href="">FANS</a></li>
            <li><a href="">NEWS</a></li>
            <li><a href="">SHOP</a></li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@use '../assets/partials/variables' as *;

    nav{
        ul{
            margin: 0;
            list-style: none;
            display: flex;
        }
        li{
            a{
                display: inline-block;
                padding: 18px;
                text-decoration: none;
                color: $third-color;
                font-size: 14px;
                font-weight: bolder;
            }
        }
    }
</style>
