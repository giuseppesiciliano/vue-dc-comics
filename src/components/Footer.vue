<template>
    <footer>
        <div class="bg-image">

            <div class="container">
                <div class="list">

                    <!-- COL-LEFT -->
                    <div class="col left">

                        <!-- DC Comics -->
                        <div class="list-name">
                            <div class="text">{{lists[0].title}}</div>
                            <ul>
                                <li v-for="(element, index) in lists[0].links" :key="index">
                                    <a href="#">{{ element.name }}</a>
                                </li>
                            </ul>
                        </div>

                        <!-- Shop -->
                        <div class="list-name">
                            <div class="text">{{lists[1].title}}</div>
                            <ul>
                                <li v-for="(element, index) in lists[1].links" :key="index">
                                    <a href="#">{{ element.name }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- END COL-LEFT -->


                    <!-- COL-CENTRAL -->
                    <div class="col central">

                        <!-- DC -->
                        <div class="list-name">
                            <div class="text">{{lists[2].title}}</div>
                            <ul>
                                <li v-for="(element, index) in lists[2].links" :key="index">
                                    <a href="#">{{ element.name }}</a>
                                </li>

                            </ul>
                        </div>
                    </div>
                    <!-- END COL-CENTRAL -->


                    <!-- COL-RIGHT -->
                    <div class="col right">

                        <!-- DC -->
                        <div class="list-name">
                            <div class="text">{{lists[3].title}}</div>
                            <ul>
                                <li v-for="(element, index) in lists[3].links" :key="index">
                                    <a href="#">{{ element.name }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- END COL-RIGHT -->
                </div>
            </div>
        </div>

        

        <div class="sign-up"></div>
    </footer>
</template>


<script>
export default {
    name: 'Footer',
    data: function() {
        return {
            lists: [
                {
                    title: 'DC COMICS',
                    links: [
                        {
                            name: 'Characters',
                            url: '#'
                        },
                        {
                            name: 'Comics',
                            url: '#'
                        },
                        {
                            name: 'Movies',
                            url: '#'
                        },
                        {
                            name: 'TV',
                            url: '#'
                        },
                        {
                            name: 'Games',
                            url: '#'
                        },
                        {
                            name: 'Videos',
                            url: '#'
                        },
                        {
                            name: 'News',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'SHOP',
                    links: [
                        {
                            name: 'Shop DC',
                            url: '#'
                        },
                        {
                            name: 'Schop DC Collectibles',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            name: 'Terms Of Use',
                            url: '#'
                        },
                        {
                            name: 'Privacy policy (New)',
                            url: '#'
                        },
                        {
                            name: 'Ad Choises',
                            url: '#'
                        },
                        {
                            name: 'Advertising',
                            url: '#'
                        },
                        {
                            name: 'Jobs',
                            url: '#'
                        },
                        {
                            name: 'Subscriptions',
                            url: '#'
                        },
                        {
                            name: 'Talent Workshops',
                            url: '#'
                        },
                        {
                            name: 'CPSC Certificates',
                            url: '#'
                        },
                        {
                            name: 'Ratings',
                            url: '#'
                        },
                        {
                            name: 'Shop Help',
                            url: '#'
                        },
                        {
                            name: 'Contact Us',
                            url: '#'
                        }
                    ]
                },
                {
                    title: 'SITES',
                    links: [
                        {
                            name: 'DC',
                            url: '#'
                        },
                        {
                            name: 'MAD Magazine',
                            url: '#'
                        },
                        {
                            name: 'DC Kids',
                            url: '#'
                        },
                        {
                            name: 'DC Universe',
                            url: '#'
                        },
                        {
                            name: 'DC Power Visa',
                            url: '#'
                        }
                    ]
                }
            ]
        }
    }
}
</script>


<style scoped lang="scss">
@import '../style/common.scss';


.bg-image {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 500px;
    background-repeat: no-repeat;
    background-size: cover;
}

.list {
    display: flex;
    padding: 50px;
    color: white;
}
.col {
    padding-right: 50px;
}
.list-name {
    padding-bottom: 30px;

    .text {
        font-size: 20px;
        font-weight: bold;
    }

    li {
        padding: 5px 0;
        color: gray;

        a {
            color: gray;
        }
    }
}

.sign-up {
    background-color: #303030;
    height: 120px;
}
</style>