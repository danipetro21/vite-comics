<script>

export default {
    name: "AppFooter",
}

</script>

<template>

    <footer>
        <div class="box">

            <div class="footer-box">


                <div class="left-box">

                    <ul>
                        <h5>DC COMICS</h5>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>

                        <ul>
                            <h5>SHOP</h5>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy(NEW)</a></li>
                        </ul>
                    </ul>

                    <ul>
                        <h5>DC</h5>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy(NEW)</a></li>
                        <li><a href="#">Ad Choise</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop help</a></li>
                        <li><a href="#">Contact US</a></li>

                    </ul>

                    <ul>
                        <h5>SITES</h5>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy(NEW)</a></li>
                        <li><a href="#">Ad Choise</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                    </ul>


                </div>


                <div class="right-box">

                    <img src="public/img/dc-logo-bg.png" alt="">

                </div>

            </div>


        </div>

        <div class="bootom-box">

            <div class="footer-bottom-box">

                <a href="">SIGN-UP NOW!</a>

                <ul>
                   <h3>FOLLOW US</h3> 
                    <li><img src="public/img/footer-facebook.png" alt=""></li>
                    <li><img src="public/img/footer-twitter.png" alt=""></li>
                    <li><img src="public/img/footer-youtube.png" alt=""></li>
                    <li><img src="public/img/footer-pinterest.png" alt=""></li>
                    <li><img src="public/img/footer-periscope.png" alt=""></li>
                </ul>
            </div>

        </div>
    </footer>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

footer {

    background-image: url("public/img/footer-bg.jpg");
    width: 100%;
    height: 500px;

}

.box {
    max-width: 1400px;
    margin: 0 auto;
    height: 100%;
}

.footer-box {
    display: flex;
}

.left-box {
    color: $primary_color;
    display: flex;
    width: 50%;


    h5 {
        font-size: 1.2rem;
    }

    li {
        margin: 5px 0;
    }

    li a {
        text-decoration: none;
        color: $secondary_color;

        &:hover {
            color: red;
        }
    }

    ul {
        margin-top: 50px;
        margin-right: 20px;
    }

}

.right-box {

    width: 50%;

    img {
        width: 90%;
        object-fit: cover;
        object-position: 0 -50px ;
    }
}

.bootom-box {
    position: absolute;
    width: 100%;
    height: 150px;
    background-color: $bg_footer_color ;
}

.footer-bottom-box{
    margin: 0 auto;
    max-width: 1400px;
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    a{
        color: $primary_color;
        text-decoration: none;
        padding: 15px;
        border: 2px $text_color solid;
    }

    ul{
        display: flex;
        align-items: center;
        gap: 20px;
        h3{
            color: $text_color;
        }
    }


}


</style>
