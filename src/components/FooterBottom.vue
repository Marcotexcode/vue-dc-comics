<template>
  
  <div class="container">
      <div class="footer-bottom">
            <button><span>sing-up now!</span></button>
            <div class="link">
                <h3>follow us</h3>
                <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
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
        background-color: #303030;
        
        .footer-bottom {
            display: flex;
            padding: 30px;
            width: $widthContainer;
            margin: 0 auto;
            justify-content: space-between;

            button {
                background-color: #303030;
                border: 2px solid $colorBlue;
                columns: white;
                padding: 10px 20px;

                span {
                    color: white;
                    font-size: 15px;
                    text-transform: uppercase;
                }
            }

            .link {
                display: flex;
                align-items: center;
                
                h3 {
                    text-transform: uppercase;
                    color: $colorBlue;
                    margin-right: 10px;
                }

                a {
                    margin: 0px 10px;
                }
            }

        }
        
    }



</style>