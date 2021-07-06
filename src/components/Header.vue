<template>
    <header>
        <div class="container header">
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
        </div>
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


    ul {
        list-style: none;

        li {
            display: inline-block;
            margin: 15px;

            &:hover,
            &.active {
                border-bottom: 3px solid $blue-dc;
            }


            a {                
                text-decoration: none; 
                text-transform: uppercase;     
                color: black;
                font-weight: 700;
                line-height: calc(150px - (3px * 2)); //border *2
                
             &:hover,
             &.active {
                    color: $blue-dc;
             }
            }


        }

    }
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: $std-height;
    //border: 1px solid black; !da togliere
}

</style>