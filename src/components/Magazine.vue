<template>
    <div class="single-magazine">
        <div class="box">
            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
        </div>

        <h5>ACTION COMICS</h5>
    </div>
</template>


<script>
export default {
    name: 'Magazine'
}
</script>


<style scoped lang="scss">
.single-magazine {
    width: calc( 100% / 6 );
    padding: 20px 0;

    .box {
        width: 200px;
        height: 200px;
        overflow: hidden;
    }
    h5 {
        padding-top: 20px;
    }
}
</style>