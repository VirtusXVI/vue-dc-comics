<template>
  <div>
    <section>
        <div class="upper-main-adjustments">
            <div class="upper-main-jumbotron">

            </div>
            <div class="container">
                <div class="cards-container">
                    <h2>ciao</h2>
                </div>
            </div>
        </div>
    </section>
    <MyCards/>
  </div>
</template>

<script>
import MyCards from "./MyCard.vue"
export default {
    name: "MyMain",
    components:{
        MyCards,
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
    .cards-container{
        padding: 3rem 0;
    }
</style>