<template>
  <div class="container">
      <div class="jumbo">
          <button>current series</button>
      </div>
  </div>
  

</template>

<script>
export default {

    name: 'Jumbotron'

}
</script>

<style lang="scss" scoped>

    @import '../style/variabili.scss';
    @import '../style/mixins.scss';

    .container {
        background-image: url('../assets/img/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 300px;

        .jumbo {
            @include containerCentral ();
            position: relative;

            button {
                @include button ($colorBlue);
                font-size: 18px;
                position: absolute;
                top: 280px;
            }
        }
    }
</style>