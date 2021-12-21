<template>
    <div class="single-magazine">
        <div class="box">
            <img :src="magazineObject.thumb" alt="">
        </div>

        <h5>{{magazineObject.series.toUpperCase()}}</h5>
    </div>
</template>


<script>
export default {
    name: 'Magazine',
    props: ['magazineObject']
}
</script>


<style scoped lang="scss">
.single-magazine {
    width: calc( 100% / 6 );
    padding-top: 50px;

    .box {
        width: 200px;
        height: 200px;
        overflow: hidden;
    }
    h5 {
        padding-top: 20px;
        margin-right: 40px;
    }
}
</style>