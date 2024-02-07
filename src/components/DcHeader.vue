<template>
    <header>
        <div class="header-container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="(voice, index) in menu_voices" :key="index">
                        <a href="#">{{ voice }}</a>
                    </li>

                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
header {
    background-color: white;

    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 60%;
        margin: 0 auto;
    }
}
</style>


<script>
export default {
    data() {
        return {
            menu_voices: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"]
        }
    }
}
</script>