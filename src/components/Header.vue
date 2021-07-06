<template>

    <div class="container">

        <header>

            <img src="../assets/img/dc-logo.png" alt="">

            <nav>

                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                </ul>

            </nav> 

        </header>

    </div>
   

</template>


<script>
export default {

    name: 'Header',

    data() {

    }

}
</script>


<style lang="scss" scope>

    @import '../style/variabili.scss';

         
    header {
        display: flex;
        justify-content: space-between;
        border: 1px solid #000;
        align-items: center;
        padding: 20px;
        width: 80%;
        margin: 0 auto;

        img {
            width: 70px;
        }

        ul {
            display: flex;      
            
            li{
                padding: 20px;
                list-style: none;

                a {
                    color: black;
                    text-decoration: none;
                    text-transform: uppercase;

                    &:hover {
                        color: $colorblue;
                        border-bottom: 3px solid $colorblue;
                        padding-bottom: 100%;
                    }
                }
            }
        }
    }

</style>