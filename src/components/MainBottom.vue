<template>

    <div class="container">

        <div class="main-bottom">

            <div v-for="(elementi, index) in box" :key="index" class="box">

                <img :src="elementi.src" :alt="elementi.nome">

                <h4>{{elementi.nome}}</h4>

            </div>

        </div>

    </div>
  
</template>

<script>

    export default {

        name:'MainBottom',

        data() {

            return {

                box: [
                    {
                        src: '../src/assets/img/buy-comics-digital-comics.png',
                        nome: 'digital comics'
                    },
                    {
                        src: 'src/assets/img/buy-comics-digital-comics.png',
                        nome: 'dc merchandise'
                    },
                    {
                        src: 'src/assets/img/buy-comics-digital-comics.png',
                        nome: 'subscription'
                    },
                    {
                        src: 'src/assets/img/buy-comics-digital-comics.png',
                        nome: 'comic shop locator'
                    },
                    {
                        src: 'src/assets/img/buy-comics-digital-comics.png',
                        nome: 'dc power visa'
                    },
                ]

            }

        }

    }

</script>

<style lang="scss" scoped>

    @import '../style/variabili.scss';

    .container {
        background-color: $colorBlue;
        

        .main-bottom {
            width: $widthContainer;
            margin: 0 auto;
            padding: 30px;
            display: flex;
            justify-content: space-between;

            .box {
                display: flex;
                align-items: center;
                img {
                    width: 70px;
                    margin-right: 10px;
                }

                h4 {
                    color: white;
                    text-transform: uppercase;
                }

            }

        }
    }



</style>