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
                                    <a href="#">{{element.name}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- END COL-RIGHT -->
                </div>
            </div>

            <div class="bg-img-dc">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>

        </div>

        
        <div class="end-footer">
            <div class="container">
                <div class="content">

                    <div class="sign-up">SIGN-UP NOW!</div>

                    <div class="social">
                        FOLLOW US
                        <div class="icons">
                            <img v-for="(logo, index) in logos" :key="index" :src="logo.logo" :alt="logo.alt">
                        </div>
                    </div>
                </div>
            </div>
        </div>
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
            ],
            logos: [
                {
                    alt: "Facebook",
                    logo: require ('../assets/img/footer-facebook.png')
                },
                {
                    alt: "Twitter",
                    logo: require ('../assets/img/footer-twitter.png')
                },
                {
                    alt: "YouTube",
                    logo: require ('../assets/img/footer-youtube.png')
                },
                {
                    alt: "Pinterest",
                    logo: require ('../assets/img/footer-pinterest.png')
                },
                {
                    alt: "Periscope",
                    logo: require ('../assets/img/footer-periscope.png')
                }
            ]
        }
    }
}
</script>


<style scoped lang="scss">
@import '../style/common.scss';
@import '../style/variables.scss';


.bg-image {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 500px;
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;
    display: flex;
    position: relative;

    .bg-img-dc {
        position: absolute;
        top: -30px;
        right: 300px;
    }
}

.list {
    display: flex;
    padding: 50px;
    color: $brand_secondary_color;
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

.end-footer {
    background-color: #303030;
}
.content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 20px;

    .sign-up {
        border: 2px solid $brand_primary_color;
        padding: 10px;
        color: $brand_secondary_color;
        margin: 30px 0;
    }

    .social {
        color: $brand_primary_color;
        font-weight: bold;
        display: flex;
        align-items: center;

        img {
            padding-left: 20px;
        }
    }
}
</style>