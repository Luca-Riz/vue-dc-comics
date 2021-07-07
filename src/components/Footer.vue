<template>
    <footer>
        <!-- inizio navbar footer -->
        <div class="main-top">
            <div class="container footer-top">
                <ul>
                    <li class="nav-footer" v-for="(link,index) in links" :key="index">
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
                    
                    <!-- inizio box singolo prodotto -->
                    <div class="box-product">
                        <h2>Dc comics</h2>
                        <ul>
                            <li v-for="(item,index) in dcComics" :key="index">
                                <a :href="item.link"> {{item.text}} </a>
                            </li>
                        </ul>
                    </div>
                    <!-- fine box singolo prodotto -->

                    <!-- inizio box singolo prodotto -->
                    <div class="box-product">
                        <h2>Shop</h2>
                        <ul>
                            <li v-for="(item,index) in shop" :key="index">
                                <a :href="item.link"> {{item.text}} </a>
                            </li>
                        </ul>
                    </div>
                    <!-- fine box singolo prodotto -->

                    <!-- inizio box singolo prodotto -->
                    <div class="box-product">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="(item,index) in dc" :key="index">
                                <a :href="item.link"> {{item.text}} </a>
                            </li>
                        </ul>
                    </div>
                    <!-- fine box singolo prodotto -->

                    <!-- inizio box singolo prodotto -->
                    <div class="box-product">
                        <h2>Sites</h2>
                        <ul>
                            <li v-for="(item,index) in sites" :key="index">
                                <a :href="item.link"> {{item.text}} </a>
                            </li>
                        </ul>
                    </div>
                    <!-- fine box singolo prodotto -->

                </nav>
                <!-- fine main nav footer -->

                <!-- logo main footer -->
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo dc bg">
                </div>
                <!-- fine logo main footer -->

            </div>
        </div>
        <!-- fine main footer -->

        <!-- inizio bottom footer -->
        <div class="main-bottom">
            <div class="container bottom-footer">

                <!-- inizio footer bottom left -->
                <div class="left pointer">
                    Sign-up now!
                </div>
                <!-- fine footer bottom left -->


                <!-- inizio footer bottom right -->
                <div class="right">
                    <div class="blue">Follow us</div>
                    <div class="social" v-for="(item,index) in social" :key="index">
                        <!-- <a :href="item.link"> {{item.text}} </a> -->
                        <img :src="item.src" :alt="item.alt">
                    </div>
                </div>
                <!-- fine footer bottom right -->


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
                    src: require('../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'DC merchandise',
                    url: '#',
                    current: false,
                    src: require('../assets/img/buy-comics-merchandise.png')                    
                },
                {
                    text: 'Subscription',
                    url: '#',
                    current: false,
                    src: require('../assets/img/buy-comics-subscriptions.png'),
                },
                {
                    text: 'Comic shop locator',
                    url: '#',
                    current: false,
                    src: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'DC power Visa',
                    url: '#',
                    current: false,
                    src: require('../assets/img/buy-dc-power-visa.svg')
                }
               
            ],

            dcComics: [
                {
                    text: 'Characters',
                    link: '#'
                },
                {
                    text: 'Comics',
                    link: '#'
                },
                {
                    text: 'Movies',
                    link: '#'
                },
                {
                    text: 'TV',
                    link: '#'
                },
                {
                    text: 'Games',
                    link: '#'
                },
                {
                    text: 'Videos',
                    link: '#'
                },
                {
                    text: 'News',
                    link: '#'
                }
            ],
                
            shop: [
                {
                    text: 'Shop DC',
                    link: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    link: '#'
                }
            ],
                
            dc: [
                {
                    text: 'Terms Of Use',
                    link: '#'
                },
                {
                    text: 'Privacy policy (New)',
                    link: '#'
                },
                {
                    text: 'Ad Choices',
                    link: '#'
                },
                {
                    text: 'Advertising',
                    link: '#'
                },
                {
                    text: 'Jobs',
                    link: '#'
                },
                {
                    text: 'Subscriptions',
                    link: '#'
                },
                {
                    text: 'Talent Workshops',
                    link: '#'
                },
                {
                    text: 'CPSC Certificates',
                    link: '#'
                },
                {
                    text: 'Rating',
                    link: '#'
                },
                {
                    text: 'Shop Help',
                    link: '#'
                },
                {
                    text: 'Contact Us',
                    link: '#'
                }
            ],
                
            sites: [
                {
                    text: 'DC',
                    link: '#'
                },
                {
                    text: 'MAD Magazine',
                    link: '#'
                },
                {
                    text: 'DC Kids',
                    link: '#'
                },
                {
                    text: 'DC Universe',
                    link: '#'
                },
                {
                    text: 'DC Power Visa',
                    link: '#'
                }
            ],

            social: [
                {
                    src: require('../assets/img/footer-facebook.png'),
                    link: '#',
                    alt: 'facebook logo'
                },
                {
                    src: require('../assets/img/footer-twitter.png'),
                    link: '#',
                    alt: 'twitter logo'
                },
                {
                    src: require('../assets/img/footer-youtube.png'),
                    link: '#',
                    alt: 'youtube logo'
                },
                {
                    src: require('../assets/img/footer-pinterest.png'),
                    link: '#',
                    alt: 'pinterest logo'
                },
                {
                    src: require('../assets/img/footer-periscope.png'),
                    link: '#',
                    alt: 'periscope logo'
                },
            ]
                

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
                width: 100%;
                list-style: none;
                display: flex;
                justify-content: space-between;

                li {
                    display: inline-block;
                    margin: 15px;
                    display: flex;
                    align-items: center;

                        img {
                            height: 3rem;
                            margin-right: 1rem;
                        }
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
    height: 400px; //! da togliere
    color: white;
    display: flex;


        .main-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            overflow: hidden;

            nav {
                height: 100%;
                display: flex;
                flex-direction: column;
                align-content: flex-start;
                flex-wrap: wrap;

                .box-product {
                    // border: 1px solid red;
                    display: inline-block;
                    margin-right: 1.5rem;

                    h2 {
                        padding: 1.25rem 0;
                        text-transform: uppercase; 
                    }

                    ul {
                        list-style: none;

                        li {
                            padding: 0.25rem 0;
                        }
                        
                        a {                
                            text-decoration: none; 
                            color: lightgrey;
                            font-weight: 300;                      
                        }
                    }
                }

            }

        }
}

.main-bottom {
    height: $std-height;
    background-color: $grey-dc;
    display: flex;
    align-items: center;

    .bottom-footer{

        display: flex;
        justify-content: space-between;
        align-items: center;
    
        .left {
            text-transform: uppercase; 
            color: white;
            padding: 15px;
            display: inline-block;
            border: 3px solid $blue-dc;
            cursor: pointer;
        }
    
        .right {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            text-transform: uppercase; 
    
            .blue{
                color: $blue-dc;
                padding: 10px;
                font-weight: 600;

            }

            .social {
                padding: 10px;
            }
    }
}
        




}

</style>