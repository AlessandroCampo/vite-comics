<template>
    <section>
        <div class="section-container">
            <div class="list-container">
                <div class="list-group">
                    <h3>
                        DC COMICS
                    </h3>
                    <ul>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                    </ul>
                    <h3>
                        SHOP
                    </h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>

                <div class="list-group">
                    <h3>
                        DC COMICS
                    </h3>
                    <ul>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                    </ul>
                </div>

                <div class="list-group">
                    <h3>
                        DC COMICS
                    </h3>
                    <ul>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                        <li>
                            Characters
                        </li>
                    </ul>
                </div>
            </div>


            <figure>

            </figure>

        </div>
    </section>
</template>

<script>
export default {
    data() {

    }
}
</script>

<style lang="scss" scoped>
section {
    background-image: url("../assets/img/footer-bg.jpg");
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-block: 3%;

    .section-container {
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-around;


        .list-container {
            display: flex;
            gap: 50px;
        }

        figure {
            background-image: url("../assets/img/dc-logo-bg.png");
            height: 250px;
            width: 250px;
            border: 2px solid red;
            background-size: cover;
        }
    }
}

.list-group {
    h3 {
        color: white;
    }

    ul {
        display: flex;
        flex-direction: column;
        gap: 5px;
        margin-top: 15px;
        list-style: none;
    }

    li {
        color: gray;
    }
}
</style>