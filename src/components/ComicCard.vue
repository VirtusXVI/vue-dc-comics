<template>
  <div>
    <div v-for="comic,index in comics" :key="index" class="card">
        <div>
            <img :src="comics[index].thumb" alt="">
        </div>
        <div>

        </div>
    </div>
  </div>
</template>

<script>
import ComicData from "../assets/dc-comics.json"
export default {
    name: "ComicCard",
    components: {
        ComicData
    },
    data () {
        return {
            comics: ComicData
        }
    }

}
</script>

<style scoped lang="scss">

</style>