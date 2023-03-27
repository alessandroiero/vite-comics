<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name: 'AppFooter'
}
</script>

<template>
    <div class="footer-bottom">
        <div class="container">
            <button class="button registrati">SIGN-UP NOW!</button>
            <div class="socials">
                <h3>FOLLOW US</h3>
                <img src="../assets/img/footer-facebook.png" alt="facebook">
                <img src="../assets/img/footer-twitter.png" alt="twitter">
                <img src="../assets/img/footer-youtube.png" alt="yt">
                <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                <img src="../assets/img/footer-periscope.png" alt="periscope logo">
            </div>
        </div>
    </div>
</template>

<style lang='scss' scoped>
@use '../assets/partials/variables' as *;

.footer-bottom {
    background-color: $third_color;
    .container {
        background-color: $third_color;
        width: 100%;
        padding: 20px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    // bottone
    button {
        color: $fourth_color;
        background-color: inherit;
        padding: 15px;
        border: 2px solid $secondary_color;
        font-weight: bolder;
    }

    .socials {
        display: flex;
        align-items: center;

        h3 {
            color: $secondary_color;
        }
        img{
            margin: 0 10px;
        }
    }
}
</style>
