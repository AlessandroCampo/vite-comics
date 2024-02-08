<template>
    <header>
        <div class="header-container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="(voice, index) in menu_voices" :key="index">
                        <a :href="voice.link" :class="voice.active ? 'active' : ''">{{ voice.name }}</a>
                    </li>

                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use "../styles/partials/mixin";
@use "../styles/partials/variables" as *;

header {
    background-color: white;

    .active {
        color: $dc_lightblue;
        border-bottom: 8px solid $dc_lightblue;
    }

    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 70%;
        margin: 0 auto;
        margin-top: 20px;
        padding-block: 15px;
        height: 14vh;
    }

    ul {
        display: flex;
        list-style: none;
        gap: 20px;
        font-weight: bold;
        font-size: 16px;
        height: 100%;

        li {
            a {
                text-decoration: none;
                color: #464646;
                padding-bottom: calc(14vh / 2 - 16px);

                &:hover {
                    color: $dc_lightblue;
                    border-bottom: 8px solid $dc_lightblue;
                }
            }
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
                { name: "COMICS", link: "#", active: true },
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