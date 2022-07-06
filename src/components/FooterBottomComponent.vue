<template>
    <section class="bottom-footer">
            <div class="container">
                <span>
                    <a href="#">SIGN-UP NOW!</a>
                </span>
                <ul>
                    <li>FOLLOW US</li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="Facebook">    
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="Twitter">    
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="Youtube">    
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">    
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="Periscope">    
                        </a>
                    </li>
                    
                </ul>
            </div>
    </section>
</template>

<script>
export default {
    name: "FooterBottomComponent"
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    section{
        background-color: $secondary-color;
    }
    .container{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        padding: 3rem;
    }
    span{
        a{
            color: white;
            border: 2px solid $primary-color;
            padding: 1rem;
        }
    }
    ul{
        display: flex;
        align-items: center;
        li{
            margin-right: 10px;
            &:first-child{
            color: $primary-color;
        }
        }
    }
</style>
