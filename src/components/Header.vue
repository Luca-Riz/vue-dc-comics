<template>
    <header>
        <a href="#">
            <img src="@/assets/img/dc-logo.png" alt="logo dc">
            <!-- oppure
            <img src="../assets/images/logo.png" alt=""> -->
        </a>
        <nav>
            <ul>
                <!-- <li v-for="(link,index) in links" :key="index" :class="{ active: link.current }"><a :href="link.url">{{ link.text }} </a></li> -->
                <!-- oppure -->
                <li v-for="(link,index) in links" :key="index" :class="link.current ? 'active' : '' "><a :href="link.url">{{ link.text }} </a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: false
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false
                },
                {
                    text: 'News',
                    url: '#',
                    current: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';
header{
    text-align: center;

    ul {
        list-style: none;

        li {
            display: inline-block;
            padding: 10px;

            a {
                color: $primary;
                text-decoration: none;
                font-size: $font_primary;
            }

             &:hover,
             &.active {
                    background-color: lightgrey;
             }

        }

    }
}

</style>