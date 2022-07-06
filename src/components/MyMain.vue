<template>
  <div>
    <section>
        <div class="upper-main-adjustments">
            <div class="container">
                <h1>-- Content Goes Here --</h1>
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
        padding: 3rem;
        background-color: black;
        color: white;
    }
</style>