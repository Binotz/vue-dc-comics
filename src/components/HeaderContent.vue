<template>
  <header>
    <div class="container">
        <!-- Logo image -->
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        <!-- menu -->
        <div class="menu-list">
            <ul>
                <li v-for="link,index in menuList" :key="index">
                    <a :href="link.link" :class="{'current': link.currentPage}">
                        {{ link.text.toUpperCase() }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
  </header>
</template>

<script>
export default {
    name:"HeaderContent",
    data(){
        return{
            menuList:[
                {
                    text: 'characters',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'comics',
                    link: '#',
                    currentPage: true,
                },                {
                    text: 'movies',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'tv',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'games',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'collectibles',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'videos',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'fans',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'news',
                    link: '#',
                    currentPage: false,
                },                {
                    text: 'shop',
                    link: '#',
                    currentPage: false,
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1rem 0;
    }
    ul{
        display: flex;
        li{
            margin-left: 1.5rem;
        }
    }
    .menu-list{
        display: flex;
        align-items: center;
        height: $menu-height;
        a{
            color: gray;
            font-weight: bold;
        }
        .current{
            color: $primary-color;
        }
    }
</style>
