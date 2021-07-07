<template>

    <div class="container">

        <div class="main-bottom">

            <div v-for="(elementi, index) in box" :key="index" class="box">

                <img :src ="elementi.src" :alt="elementi.nome">

                <h4>{{elementi.nome}}</h4>

            </div>

        </div>

    </div>
  
</template>

<script>

    export default {

        name:'Sezione2',

        data() {

            return {

                box: [
                    {
                        src: require('../assets/img/buy-comics-digital-comics.png'),
                        nome: 'digital comics'
                    },
                    {
                        src: require('../assets/img/buy-comics-merchandise.png'),
                        nome: 'dc merchandise'
                    },
                    {
                        src: require('../assets/img/buy-comics-subscriptions.png'),
                        nome: 'subscription'
                    },
                    {
                        src: require('../assets/img/buy-comics-shop-locator.png'),
                        nome: 'comic shop locator'
                    },
                    {
                        src: require('../assets/img/buy-dc-power-visa.svg'),
                        nome: 'dc power visa'
                    },
                ]

            }

        }

    }

</script>

<style lang="scss" scoped>

    @import '../style/variabili.scss';
    @import '../style/mixins.scss';

    .container {
        background-color: $colorBlue;
        

        .main-bottom {
            @include containerCentral ();
            display: flex;
            justify-content: space-between;

            .box {
                display: flex;
                align-items: center;
                img {
                    width: 40px;
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