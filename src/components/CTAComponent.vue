<template>
    <section class="cta">
        <div class="container">
            <ul>
                <li v-for="icon,index in icons" :key="index">
                    <img :src="icon.iconPath" :alt="icon.iconAlt">
                    <a :href="icon.link">{{ icon.text.toUpperCase() }}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "CTAComponent",
    data(){
        return{
            icons:[
                {
                    text: 'digital comics',
                    iconPath: require('../assets/img/buy-comics-digital-comics.png'),
                    link:'#',
                    iconAlt: 'Buy Digital'
                },                
                {   text: 'dc merchandise',
                    iconPath: require('../assets/img/buy-comics-merchandise.png'),
                    link:'#',
                    iconAlt: 'Buy Merchandise'
                },                
                {
                    text: 'subscription',
                    iconPath: require('../assets/img/buy-comics-subscriptions.png'),
                    link:'#',
                    iconAlt: 'Buy Subscription'
                },                
                {
                    text: 'comic shop location',
                    iconPath: require('../assets/img/buy-comics-shop-locator.png'),
                    link:'#',
                    iconAlt: 'Shop Locator'
                },                
                {
                    text: 'dc power visa',
                    iconPath: require('../assets/img/buy-dc-power-visa.svg'),
                    link:'#',
                    iconAlt: 'DC Power Visa'
                },

            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';
    section{
        background-color: $primary-color;
    }
    ul{
        display: flex;
        justify-content: space-between;
        padding: 3rem 0;
    }
    li{
        display: flex;
        align-items: center;
        a{
            color: white;
            line-height: 100%;
        }
    }
    img{
        height: 50px;
        margin-right: 15px;
    }
</style>
