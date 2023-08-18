<template>
    <div class="header">
        <section class="logo">
            <img src="" alt="">
            <p>WeatherFred</p>
        </section>
        <nav>
            <ul>
                <li>
                    <a href="">Search</a>
                </li>
                <li>
                    <a href="">Overview</a>
                </li>
                <li>
                    <a href="">Help</a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>

    export default {

        name: "HeaderView",
        props: {
            msg: String
        }
    }

</script>


<style scoped>
    .header {
        height: 26px;
        display: flex;
        margin: 0;
        padding: 20px 0 5px 0;
        justify-content: space-between;
        background-color: blueviolet;
        color: aliceblue;
    }

    .logo {
        min-width: 100px;
        display: flex;
    }

    .logo > * {
        width: 20px;
        height: 20px;
        margin: 0;
        padding-left: 5px;
    }

    ul {
        min-width: 300px;
        display: flex;
        justify-content: space-evenly;
        margin: 0;
        padding: 0 50px 0 0;
        list-style: none;
        
    }

    ul a {
        color: azure;
    }
</style>