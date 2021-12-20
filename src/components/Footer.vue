<template>
    <footer>
        <div class="bg-image"></div>
        <div class="container"></div>
        <div class="sign-up"></div>
    </footer>
</template>


<script>
export default {
    name: 'Footer'
}
</script>


<style scoped lang="scss">
.bg-image {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 500px;
    background-repeat: no-repeat;
    background-size: cover;
}

.sign-up {
    background-color: #303030;
    height: 120px;
}
</style>