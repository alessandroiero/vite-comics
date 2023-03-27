<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name: 'AppDescription'
}
</script>

<template>
    <section class="description">
        <div class="container blue">
            <ul>
                <li>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="buy comics">
                    <span>DIGITAL COMICS</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
                    <span>DC MERCHANDISE</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                    <span>SUBSCRIPTION</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="shop location">
                    <span>COMIC SHOP LOCATOR</span>
                </li>
                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="visa">
                    <span>DC POWER VISA</span>
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/partials/variables' as *;

.description {
    background-color: $secondary_color;
    padding: 3.125rem;
    color: $fourth_color;
    .container.blue {
        ul {
            display: flex;
            justify-content: space-around;
            li {
                cursor: pointer;
                display: flex;
                align-items: center;
                span{
                margin-left: 10px;
                }
                img {
                    width: 50px;
                }
            }
        }
    }
}
</style>
