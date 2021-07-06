<template>
    <footer>
        <div class="container footer">
            <ul>
                <li v-for="(link,index) in links" :key="index">
                    <img :src="link.src" alt="#">
                    <a :href="link.url"> {{ link.text }} </a>
                </li>
            </ul>
        </div>
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
               
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

footer{
    background-color: $blue-dc;
    height: $std-height;

    .footer {
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


</style>