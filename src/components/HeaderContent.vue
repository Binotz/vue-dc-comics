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
                <li v-for="link,index in menuList" :key="index" :class="{'current': link.currentPage}">
                    <a :href="link.link">
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

    header {
        min-height: $menu-height;
    }
    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 100%;
    }
    ul{
        display: flex;
        align-items: center;
        height: 100%;
        li{
            margin-left: 1.5rem;
            height: $menu-height;
            display: flex;
            align-items: center;
            &.current{
                border-bottom: 5px solid $primary-color;
                //Fix the border bottom offset
                a{
                    color: $primary-color;
                    margin-top: 5px;
                }
            }
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
