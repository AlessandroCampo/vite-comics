<template>
    <nav>
        <div class="nav-container">
            <figure v-for="(voice, index) in data_voices" :key="index">
                <img :src="getImagePath(voice.src)" alt="voice.text">
                <span>
                    {{ voice.text }}
                </span>
            </figure>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            data_voices: [
                {
                    text: "DIGITAL COMICS",
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    text: "DC MERCHANDISE",
                    src: "buy-comics-merchandise.png"
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    src: "buy-comics-shop-locator.png"
                },
                {
                    text: "SUBSCRIPTION",
                    src: "buy-comics-subscriptions.png"
                },
                {
                    text: "DC POWER VISA",
                    src: "buy-dc-power-visa.svg"
                },
            ],

        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href
        }
    }
}
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

nav {
    background-color: $dc_lightblue;
}

.nav-container {
    color: white;
    display: flex;
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    gap: 35px;
    padding-block: 50px;


    figure {
        display: flex;
        align-items: center;
        gap: 10px;

        img {
            width: 40px;
        }
    }
}
</style>