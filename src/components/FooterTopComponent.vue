<template>
  <section class="footer">
    <div class="container">
        <div class="footer-top">
            <div class="first-column">
                <!-- DC COMICS menu -->
                <ul class="footer-dc-comics">
                    <li>DC COMICS</li>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>
                <!-- SHOP -->
                <ul class="footer-shop">
                    <li>SHOP</li>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
            </div>
            <div class="second-column">
                <!-- DC -->
                <ul class="dc">
                    <li>DC</li>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Ad Choises</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Rating</a></li>
                    <li><a href="#">Shoop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="third-column">
                <ul class="sites">
                    <li>SITES</li>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Vise</a></li>
                </ul>
            </div>
            <!-- logo -->
            <img src="../assets/img/dc-logo-bg.png" alt="dc logo bg">
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name:"FooterComponent"
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    section{
        height: 482px;
        padding: 2rem;
        background-image: url('../assets/img/footer-bg.jpg');
        position: relative;
        overflow: hidden;
    }
    ul{
        margin-bottom: 2rem;
    }
    li{
        color: white;
        margin-bottom: .5rem;
        &:first-child{
            font-weight: bold;
            margin-bottom: 1rem;
        }
        a{
        color: gray;
        }
    }
    img{
        position: absolute;
        top: -3rem;
        right: 10rem;
    }
    .footer-top{
        display: flex;
        gap: 3rem;
        padding: 2rem 0;
    }
</style>
