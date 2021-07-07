<template>

    <div class="container">

        <div class="main-top">

            <div class="box">

                <ElementCard v-for="(card,index) in cards" :key="index" :dettagli="card"/>

            </div>

            <div class="bottone">

                <button>load more</button>

            </div>

        </div>

    </div>
    
</template>


<script>

    import ElementCard from '@/components/ElementCard.vue';
    import CardItems from '@/data/CardItems.js';

    export default {

        name: 'Sezione1',

        components: {

            ElementCard

        },

        data() {

            return{

                cards: CardItems

            }


        }

    }

</script>


<style lang="scss" scoped>

    @import '../style/variabili.scss';
    @import '../style/mixins.scss';

    .container {
        background-color: #1c1c1c;

        .main-top {
            @include containerCentral ();
    
            .box {
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
            }

            .bottone {
                margin: 30px 0px;
                text-align: center;

                button {
                    @include button ($colorBlue);
                }
            }

        }

    }

</style>