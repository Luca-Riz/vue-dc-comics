<template>
    <footer>
        <!-- inizio navbar footer -->
        <div class="main-top">
            <div class="container footer-top">
                <ul>
                    <li v-for="(link,index) in links" :key="index">
                        <img :src="link.src" alt="#">
                        <a :href="link.url"> {{ link.text }} </a>
                    </li>
                </ul>
            </div>
        </div>
        <!-- fine navbar footer -->

        <!-- inizio main footer -->
        <div class="main-main-footer">
            <div class="container main-footer">
                <!-- inizio main nav footer -->
                <nav>
                    <h4>Dc comics</h4>
                    <ul>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                    </ul>

                    <h4>Shop</h4>
                    <ul>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                    </ul>

                    <h4>Dc</h4>
                    <ul>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                    </ul>

                    <h4>Sites</h4>
                    <ul>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Characters</a></li>
                    </ul>
                </nav>
                <!-- fine main nav footer -->

                <!-- logo main footer -->
                <div class="logo"></div>
                <!-- fine logo main footer -->

            </div>
        </div>
        <!-- fine main footer -->

        <!-- inizio bottom footer -->
        <div class="main-bottom">
            <div class="container bottom-footer">


            </div>
        </div>
        <!-- fine bottom footer -->


    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            links: [
                {
                    text: 'Digital comics',
                    url: '#',
                    current: false,
                    src: '../assets/img/buy-comics-digital-comics.png'
                    //! da sistemare tutti url
                },
                {
                    text: 'DC merchandise',
                    url: '#',
                    current: false,
                    src: '../assets/img/buy-comics-digital-comics.png'                    
                },
                {
                    text: 'Subscription',
                    url: '#',
                    current: false,
                    src: '../assets/img/buy-comics-digital-comics.png'
                },
                {
                    text: 'Comic shop locator',
                    url: '#',
                    current: false,
                    src: '../assets/img/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC power Visa',
                    url: '#',
                    current: false,
                    src: '../assets/img/buy-comics-digital-comics.png'
                }
               
            ],

            // nav1: [
            //     {text: Characters},
            //     {text: Comics},
            //     {text: Movies},
            //     {text: TV},
            //     {text: Games},
            //     {text: Videos},
            //     {text: News}
            // ]

        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.main-top{
    background-color: $blue-dc;
    height: $std-height;

    .footer-top {
        height: 100%;
        display: flex;
        justify-content: space-around;
        align-items: center;

            ul {
                list-style: none;

                li {
                    display: inline-block;
                    margin: 15px;
                    }

                a {                
                    text-decoration: none; 
                    text-transform: uppercase;     
                    color: white;
                    font-weight: 700;                      
                }
            }    
    }
}

.main-main-footer {
    background-image: url("../assets/img/footer-bg.jpg");
    // height: 500px; //! da togliere
    color: white;

        h4 {
            padding: 10px 0;
            text-transform: uppercase; 
        }
        ul {
            list-style: none;
            
            a {                
                text-decoration: none; 
                color: white;
                font-weight: 300;                      
                }
}

.main-bottom {
    height: $std-height;
    background-color: $grey-dc;
    }
}

</style>