<template>
    <div class="card">
        <img :src="comicThumb" alt="">
        <h3> {{ comicTitle }} </h3>
    </div>
</template>
<script>
export default {
    name: "DcCard",
    props: {
        comicTitle: String,
        comicThumb: String
    }
}
</script>
<style lang="scss"scoped>
.card {
    width: calc(100% / 6);
    display: flex;
    flex-direction: column;
    gap: 10px;
    align-items: start;

    img {
        width: 100%;
        height: 200px;
    }

    h3 {
        font-size: 13px;
        text-transform: uppercase;
    }
}
</style>