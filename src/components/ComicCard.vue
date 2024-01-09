<script>
export default {
    props: {
        comic: Object
    }
}
</script>
<template lang="">
    <div class="card">
        <div class="img-container">
            <img :src="comic.thumb" alt="">
        </div>
        <div class="text-container">
            {{comic.series}}
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card {
    width: calc(100%/6 - 20px);
    height: 250px;
    overflow: hidden;
    margin: 10px;

    .img-container {
        overflow: hidden;
        height: 80%;
        width: 100%;

        img {
            width: 100%;
        }
    }

    .text-container {
        padding: 10px 0;
    }


}
</style>