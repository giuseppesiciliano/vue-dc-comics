<template>
    <header>
        <div class="container">
            <div class="content">
                <img class="logo" src="../assets/img/dc-logo.png" alt="DC Logo">

                <!-- Menu -->
                <nav>
                    <ul>
                        <li v-for="(link, index) in links" :key="index" :class="{'currentLink': index === currentLink}">
                            <a :href="link.url">{{ link.text }}</a>
                        </li>
                    </ul>
                </nav>
                
            </div>
        </div>
    </header>
</template>


<script>
export default {
    name: 'Header',
    data: function() {
        return {
            currentLink: 1,
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'TV',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: 'false'
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: 'false'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';


header {
    height: 130px;
    background-color: white;
}

.content {
    line-height: 125px;
}

.logo {
    position: relative;
    top: 15px;
    width: 100px;
    float: left;
}

// Menu
nav {
    float: right;
}
ul {
    display: flex;
}
li {
    padding: 0 30px;

    &.currentLink {
        border-bottom: 5px solid $brand_primary_color;
        a {
            color: $brand_primary_color;
        }
    }
}
li:hover {
    border-bottom: 5px solid $brand_primary_color;
    a {
        color: $brand_primary_color;
    }
}
a {
    color: black;
    font-weight: bold;
}
</style>