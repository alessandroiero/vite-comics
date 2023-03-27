<script>
// dobbiamo esportarlo per poterlo importare
export default {
    name: 'AppCards',
    data() {
        return {
            cards: [
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/seed/picsum/200/200",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }

}
</script>

<template>
    <div class="container">
        <button class="btn">CURRENT SERIES</button>
        <div class="cards">
            <div class="card" v-for="card in cards">
                <img :src="card.thumb" :alt="card.series">
                <h3>{{ card.series }}</h3>
            </div>
        </div>
        <div class="button-container">
            <button class="btn-load-more">LOAD MORE</button>
        </div>
    </div>
</template>

<!-- Stile -->
<style lang="scss" scoped>
@use '../assets/partials/variables' as *;

.container {
    .cards {
        padding-top: 50px;
        display: flex;
        flex-wrap: wrap;
    }

    .btn {
        padding: 15px 25px;
        border: none;
        transform: translateY(-20px);
        background-color: $secondary_color;
        color: $fourth_color;
    }

    .button-container {
        display: flex;
        justify-content: center;
        font-weight: bold;
        .btn-load-more {
            background-color: $secondary_color;
            color: $fourth_color;
            border: none;
            margin: 30px 0 30px 0;
            padding: 15px 50px;
            font-weight: bold;
        }
    }

    .card {
        width: calc(100% / 6);
        height: 170px;
        padding: 10px 10px;
        margin-bottom: 50px;

        h3 {
            color: $fourth_color;
            margin-top: 10px;
            font-size: 14px;
        }
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}</style>