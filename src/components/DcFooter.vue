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
                            Comics
                        </li>
                        <li>
                            Movies
                        </li>
                        <li>
                            TV
                        </li>
                        <li>
                            Games
                        </li>
                        <li>
                            Videos
                        </li>
                        <li>
                            News
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
                        DC
                    </h3>
                    <ul>
                        <li>
                            Terms Of Use
                        </li>
                        <li>
                            Privacy policy (new)
                        </li>
                        <li>
                            Ad choices
                        </li>
                        <li>
                            Advertising
                        </li>
                        <li>
                            Jobs
                        </li>
                        <li>
                            Subscriptions
                        </li>
                        <li>
                            Talent Workshops
                        </li>
                        <li>
                            CPSC Certificates
                        </li>
                        <li>
                            Ratings
                        </li>
                        <li>
                            Shop help
                        </li>
                        <li>
                            Contact us
                        </li>
                    </ul>
                </div>

                <div class="list-group">
                    <h3>
                        SITES
                    </h3>
                    <ul>
                        <li>
                            DC
                        </li>
                        <li>
                            MAD Magazine
                        </li>
                        <li>
                            DC Kids
                        </li>
                        <li>
                            DC Universe
                        </li>
                        <li>
                            DC Power Visa
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


    .section-container {
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;


        .list-container {
            padding-block: 1%;
            display: flex;
            gap: 20px;
        }

        figure {
            background-image: url("../assets/img/dc-logo-bg.png");
            width: 650px;
            height: 350px;
            background-position: center;
            background-repeat: no-repeat;
        }
    }
}

.list-group {
    font-size: 12px;

    h3 {
        color: white;
        margin-top: 30px;
        font-size: 18px;
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