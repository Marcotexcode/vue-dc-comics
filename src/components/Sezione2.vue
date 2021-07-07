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

    import ShopItems from '@/data/ShopItems.js';

    export default {

        name:'Sezione2',

        data() {

            return {

                box: ShopItems

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