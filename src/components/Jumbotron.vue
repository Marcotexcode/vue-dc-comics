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


    .container {
        background-image: url('../assets/img/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 300px;

        .jumbo {
            width: $widthContainer;
            margin: 0 auto;
            position: relative;

            button {
                border: none;
                color: white;
                background-color: $colorBlue;
                text-transform: uppercase;
                padding: 10px;
                font-size: 18px;
                position: absolute;
                top: 280px;
            }
        }
    }
</style>