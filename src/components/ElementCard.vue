<template>

        <div class="box">
            <img :src="dettagli.thumb" :alt="dettagli.series">
            <span>{{dettagli.series}}</span>
        </div>

</template>


<script>

export default {

    name: 'ElementCard',

    props: ['dettagli']

}

</script>


<style lang="scss" scoped>

    .box {
            width: 150px;
            margin: 40px 20px;
            height: 150px;

        img {
            width: 100%;
            height: 100%;
            display: block;
        }

        span {
            margin: 10px 0px;
            color: white;
        }
    }
     

</style>