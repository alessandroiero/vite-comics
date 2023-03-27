<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name: 'AppFooterList'
}
</script>

<template>
    <section class="faq">
        <div class="container footer-list">
            <nav class="lista">
                <div class="list-left">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="list-center">
                    <h3>DC</h3>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="list-right">
                    <h3>SITE</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </nav>
        </div>
    </section>
</template>

<style lang='scss' scoped>
@use '../assets/partials/variables' as *;


.faq {
    background: url('../assets/img/footer-bg.jpg');
    background-size: cover;  
    .footer-list {
        .lista {
            background-image: url(../assets/img/dc-logo-bg.png);
            height: 100%;
            background-repeat: no-repeat;
            background-position: right;
        }

        .lista {
            display: flex;
            padding-top: 1.25rem;
            div {
                margin: 15px;

                h3 {
                    color: $fourth_color;
                    margin: 5px 0;
                }

                ul {
                    li {
                        list-style: none;
                        font-size: 12px;
                        cursor: pointer;
                        padding: 5px 0;
                        color: grey;
                        &:hover {
                            color: $fourth_color;
                        }
                    }
                }
            }
        }
    }
}
</style>
