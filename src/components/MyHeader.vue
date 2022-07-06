<template>
  <div class="container">
    <div class="header-adjustments">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        <nav class="nav">
            <ul>
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
            </ul>
        </nav>
    </div>
  </div>
</template>

<script>

export default {
    name: "MyHeader",
}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import '../style/common.scss';
    .header-adjustments{
        height: 150px;
        padding: 1rem 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .logo{
        width: 30%;
    }
    .nav{
        width: 50%;
    }
    .nav ul{
        display: flex;
        align-items: center;
        justify-content: space-between;
        border-bottom: 3px solid transparent;
        height: 100%;
    }
    .active{
        border-bottom: 3px solid $brand_main_color;
        color: $brand_main_color;
    }
    li{
        font-size: 0.8rem;
        font-weight: bold;
        height: 100%;
    }
    img{
        height: 80%;
    }
</style>