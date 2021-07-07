<template>

    <div class="container">

        <div class="main-top">

            <h2>Content goes here</h2>

        </div>

    </div>
    
</template>

<script>

    export default {

        name: 'Sezione1'

    }

</script>

<style lang="scss" scoped>

    @import '../style/variabili.scss';

    .container {
        background-color: black;

        .main-top {
            width: $widthContainer;
            margin: 0 auto;
            padding: 40px 0px;

            h2 {
                color: white;
            }
        }

    }
    
    

</style>