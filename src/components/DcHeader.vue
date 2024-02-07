<template>
    <header>
        <div class="header-container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="(voice, index) in menu_voices" :key="index">
                        <a :href="voice.link">{{ voice.name }}</a>
                    </li>

                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use "../styles/partials/mixin";

header {
    background-color: white;

    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 70%;
        margin: 0 auto;
        margin-top: 20px;
        padding-block: 15px;
    }

    ul {
        display: flex;
        list-style: none;
        gap: 20px;
        font-weight: bold;
        font-size: 13px;

        a {
            text-decoration: none;
            color: #464646;
        }
    }


}
</style>


<script>
export default {
    data() {
        return {
            menu_voices: [
                { name: "CHARACTERS", link: "#", active: false },
                { name: "COMICS", link: "#", active: false },
                { name: "MOVIES", link: "#", active: false },
                { name: "TV", link: "#", active: false },
                { name: "GAMES", link: "#", active: false },
                { name: "COLLECTIBLES", link: "#", active: false },
                { name: "VIDEOS", link: "#", active: false },
                { name: "FANS", link: "#", active: false },
                { name: "NEWS", link: "#", active: false },
                { name: "SHOP", link: "#", active: false }
            ]
        }
    }
}
</script>