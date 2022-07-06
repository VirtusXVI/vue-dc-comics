<template>
  <div>
    <section>
        <div class="upper-main-adjustments">
            <div class="container">
                <h1>-- Content Goes Here --</h1>
            </div>
        </div>
    </section>
    <section>
        <div class="lower-main-adjustments">
            <div class="container">
                <MyCard/>
            </div>
        </div>
    </section>
  </div>
</template>

<script>
import MyCard from "./MyCard.vue"
export default {
    name: "MyMain",
    MyCard,
}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import '../style/common.scss';
    .upper-main-adjustments{
        padding: 3rem;
        background-color: black;
        color: white;
    }
    .lower-main-adjustments{
        padding: 3rem;
        background-color: $brand_main_color;
        color: white;
    }
</style>