<template>
  <div>
    <section>
        <div class="upper-main-adjustments">
            <div class="upper-main-jumbotron">

            </div>
            <div class="container">
                <div class="comics-container">
                    <div class="label">
                        <span>CURRENT SERIES</span>
                    </div>
                    <div class="cards-container">
                        <ComicCard />
                    </div>
                </div>
            </div>
        </div>
    </section>
    <MyCards/>
  </div>
</template>

<script>
    import MyCards from "./MyCard.vue"
    // import ComicData from "../assets/dc-comics.json"
    import ComicCard from "./ComicCard.vue"
    export default {
        name: "MyMain",
        components:{
            MyCards,
            // ComicData,
            ComicCard
        }
}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import '../style/common.scss';
    .upper-main-adjustments{
        background-color: black;
        color: white;
    }
    .upper-main-jumbotron{
        background-image: url(../assets/img/jumbotron.jpg);
        height: 400px;
    }
    .comics-container{
        padding: 3rem 0;
        position: relative;
    }
    // COMICS CARDS SECTION
    .label{
        display: inline-block;
        padding: 0.7rem 1.3rem;
        background-color: $brand_main_color;
        position: absolute;
        top: -30px;
        left: 0;
    }
    .label span{
        font-size: 1.6rem;
        font-weight: bold;
    }
    // COMICS
    .cards-container{
        width: 97%;
        margin: 0 auto;
    }
</style>