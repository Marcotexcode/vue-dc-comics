<template>

    <div class="container">

        <header>

            <img src="../assets/img/dc-logo.png" alt="">

            <nav>

                <ul>

                    <li v-for="(link, index) in links" :key="index">

                        <a :class="link.type == true ? 'active' : ' ' "  :href="link.url">{{link.text}}</a>

                    </li>
                    
                </ul>

            </nav> 

        </header>

    </div>
   

</template>


<script>

    import MenuItems from '@/data/MenuItems.js';


export default {

    name: 'Header',

    data() {

        return {

            links: MenuItems

        }

    }

}
</script>


<style lang="scss" scoped>

    @import '../style/variabili.scss';
    @import '../style/mixins.scss';
         
    header {
        @include containerCentral ();
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 90px;

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
                    font-size: 13px;
                    padding-bottom: 33px;

                    &:hover, &.active {
                        color: $colorBlue;
                        border-bottom: 3px solid $colorBlue;
                    }
                }
            }
        }
    }

</style>