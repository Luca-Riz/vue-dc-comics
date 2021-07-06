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

            dcComics : [
                {
                    text : 'Characters',
                    link : '#'
                },
                {
                    text : 'Comics',
                    link : '#'
                },
                {
                    text : 'Movies',
                    link : '#'
                },
                {
                    text : 'TV',
                    link : '#'
                },
                {
                    text : 'Games',
                    link : '#'
                },
                {
                    text : 'Videos',
                    link : '#'
                },
                {
                    text : 'News',
                    link : '#'
                }
            ],
                
            shop : [
                {
                    text : 'Shop DC',
                    link : '#'
                },
                {
                    text : 'Shop DC Collectibles',
                    link : '#'
                }
            ],
                
            dc: [
                {
                    text : 'Terms Of Use',
                    link : '#'
                },
                {
                    text : 'Privacy policy (New)',
                    link : '#'
                },
                {
                    text : 'Ad Choices',
                    link : '#'
                },
                {
                    text : 'Advertising',
                    link : '#'
                },
                {
                    text : 'Jobs',
                    link : '#'
                },
                {
                    text : 'Subscriptions',
                    link : '#'
                },
                {
                    text : 'Talent Workshops',
                    link : '#'
                },
                {
                    text : 'CPSC Certificates',
                    link : '#'
                },
                {
                    text : 'Rating',
                    link : '#'
                },
                {
                    text : 'Shop Help',
                    link : '#'
                },
                {
                    text : 'Contact Us',
                    link : '#'
                }
            ],
                
            sites : [
                {
                    text : 'DC',
                    link : '#'
                },
                {
                    text : 'MAD Magazine',
                    link : '#'
                },
                {
                    text : 'DC Kids',
                    link : '#'
                },
                {
                    text : 'DC Universe',
                    link : '#'
                },
                {
                    text : 'DC Power Visa',
                    link : '#'
                }
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
    height: 450px; //! da togliere
    color: white;
    display: flex;

        .main-footer {
            height: 100%;

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
}

</style>