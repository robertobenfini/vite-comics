<script>

</script>

<template>

    <footer>
    
        <div class="container">
            <div class="row">
                <div class="bg_dc">
                    <ul>
                        <li><h4>DC COMICS</h4></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                        <li><h4>SHOP</h4></li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
    
                    <ul>
                        <li><h4>DC</h4></li>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
    
                    <ul>
                        <li><h4>SITES</h4></li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="container_3">
            <div class="row">
                <div class="sign"><a href="#">SIGN-UP NOW!</a></div>
                <div class="social">
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="../assets/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/footer-periscope.png" alt=""></a>
                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use '../styles/partials/mixins' as *;

    .row{
        @include flex_between;
    }
    
    .container{
        background-image: url(../assets/footer-bg.jpg);

        .bg_dc{
            display: flex;
            background-image: url(../../public/dc-logo-bg.png);
            width: 100%;
            background-repeat: no-repeat;
            background-position: right center;

            ul{
                margin: 30px 20px 50px 0;
            }

        }

        li{
            a{
                color: #7F7F7F;
                font-size: 11px;
            }
            
            h4{
                color: white;
                margin: 10px 0;
            }
        }
    }

    .container_3{
        background-color: #303030;

        .sign{
            @include flex_center;
            
            a{
                color: white;
                padding: 10px;
                border: 2px solid $color_blu;
            }

        }

        .social{
            padding: 35px 0 35px 0;
            @include flex_center;

            h3{
                color: $color_blu;
                margin-right: 20px;
            }

            a{
                margin-left: 20px;
            }
        }

    }
</style>