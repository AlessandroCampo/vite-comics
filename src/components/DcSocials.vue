<template>
    <section>
        <div class="bottom-container">
            <button>
                SIGN-UP NOW!
            </button>
            <div class="socials-container">
                <h2>FOLLOW US</h2>
                <div class="icons-container">
                    <img :src=generateSrc(icon) alt="" v-for="(icon, index) in socials" :key="index">
                </div>

            </div>

        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            socials: ["facebook", "periscope", "pinterest", "twitter", "youtube"]
        }
    },
    methods: {
        generateSrc(string) {
            return `/src/assets/img/footer-${string}.png`
        }
    }
}

</script>

<style lang="scss" scoped>
section {
    display: flex;
    align-items: center;
    background-color: #303030;
    padding-block: 25px;
}

.bottom-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 70%;
    margin: 0 auto;
}

img {
    width: 35px;
}

button {
    background-color: transparent;
    padding: 10px;
    border: 1px solid #0282f9;
    color: white;
    font-weight: bold;
    font-size: 16px;
}

.socials-container {
    display: flex;
    align-items: center;
    gap: 15px;
    color: #0282f9;

    .icons-container {
        display: flex;
        gap: 12px;
    }
}
</style>