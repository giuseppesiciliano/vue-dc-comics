<template>
    <div class="preefoter">
        <div class="container">
            <div class="content">

                <div v-for="(service,index) in services" :key="index" class="service">
                    <img :src="service.logo" alt="">
                    <div class="service-text">{{ service.text }}</div>
                </div>

            </div>

        </div>
    </div>
</template>


<script>
export default {
    name: 'PreFooter',
    data: function() {
        return {
            services: [
                {
                    text: 'DIGITAL COMICS',
                    logo: require ('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    text: 'DC MERCHANDISE',
                    logo: require ('../assets/img/buy-comics-merchandise.png')
                },
                {
                    text: 'SUBSCRIPTION',
                    logo: require ('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    logo: require ('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'DC POWER VISA',
                    logo: require ('../assets/img/buy-comics-merchandise.png')
                },
            ]
        }
    }
}
</script>


<style scoped lang="scss">
@import '../style/variables.scss';
.preefoter {
    background-color: $brand_primary_color;
}
.content {
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.service {
    display: flex;
    align-items: center;
    padding: 50px 0;

    img {
        width: 60px;
    }

    .service-text {
        color: white;
        padding-left: 18px;
    }
}
</style>
