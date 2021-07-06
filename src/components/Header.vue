<template>

    <header>

        <img src="../assets/img/dc-logo.png" alt="">

        <nav>

            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
                <li><a href="#">Home</a></li>
            </ul>

        </nav> 

    </header>

</template>


<script>
export default {

    name: 'Header',

    data() {

    }

}
</script>


<style lang="scss" scope>

    header {
        display: flex;
        justify-content: space-around;
        border: 1px solid #000;

        ul {
            display: flex;
            align-items: center;
            
            li{
                padding: 20px;
                list-style: none;

                a {
                    color: black;
                    text-decoration: none;

                    &:hover {
                        color: blue;
                        border-bottom: 3px solid blue;
                        padding-bottom: 100%;
                    }
                }
            }
        }
    }

</style>