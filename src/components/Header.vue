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
export default {

    name: 'Header',

    data() {

        return {

            links: [

                {
                    text: 'characters', 
                    url: '#',
                    type: false
                },
                {
                    text: 'comics', 
                    url: '#',
                    type: true
                },
                {
                    text: 'movies', 
                    url: '#',
                    type: false
                },
                {
                    text: 'tv', 
                    url: '#',
                    type: false
                },
                {
                    text: 'games', 
                    url: '#',
                    type: false
                },
                {
                    text: 'collectibles', 
                    url: '#',
                    type: false
                },
                {
                    text: 'videos', 
                    url: '#',
                    type: false
                },
                {
                    text: 'fans', 
                    url: '#',
                    type: false
                },
                {
                    text: 'news', 
                    url: '#',
                    type: false
                },
                {
                    text: 'shop', 
                    url: '#',
                    type: false
                },
            ]

        }

    }

}
</script>


<style lang="scss" scope>

    @import '../style/variabili.scss';

         
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;
        width: $widthContainer;
        margin: 0 auto;
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
                    padding-bottom: 100%;

                    &:hover, &.active {
                        color: $colorBlue;
                        border-bottom: 3px solid $colorBlue;
                    }
                }
            }
        }
    }

</style>