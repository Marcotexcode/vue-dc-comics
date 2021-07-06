<template>

    <div class="container">
        <div class="container2">
            <div class="footer-top">

                <div class="list">
                    <h3>dc comics</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h3>shop</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collections</li>
                    
                    </ul>
                </div>
                <div class="list">
                    <h3>dc</h3>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talentr Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="list">
                    <h3>sites</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>Power Visa</li>
                    </ul>
                </div>
                <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->

            </div>

        </div>
        
    </div>
  

</template>

<script>

export default {

    name: 'FooterTop'

}

</script>

<style lang="scss" scoped>

    @import '../style/variabili.scss';

    .container {
        background-image: url('../assets/img/footer-bg.jpg');
        
        height: 400px;
        
        .container2 {
            background-image: url('../assets/img/dc-logo-bg.png');
            height: 100%;
            background-position: 80% 50%;
            background-repeat: no-repeat;

            .footer-top {
                width: $widthContainer;
                margin: 0 auto;
                display: flex;
                position: relative;

                .list {
                    margin: 0px 20px;
                    
                    h3 {
                    color: white;
                    margin: 20px 0px;
                    text-transform: uppercase;
                    }

                    ul {
                        list-style: none;
                        color: rgb(136, 136, 136);

                    }

                }

                img {   
                    width: 600px;
                    position: absolute;
                    top: -130px;
                    right: 60px;
                    backface-visibility: hidden;
                }

            }
            

        }
 
       

       
    }




</style>