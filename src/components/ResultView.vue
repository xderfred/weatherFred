<template>
    <div class="result">
        <div class="infowindow">
            <img src="" alt="city-picture">
            <section class="forecast">forecast</section>
            <section class="marine-weather">marine weather</section>
            <section class="historical-weather">historical weather</section>
            <section class="weather-alerts">weather alerts</section>
            <section class="air-quality">air quality</section>
            <section class="astronomy">astronomy</section>
        </div>
    </div>
</template>

<script>

    import { ref } from "vue"

    export default {

        setup() {
            const isResult = ref(true)

            return {
                isResult
            }
        },

        name: "ResultView",
        props: {
            msg: String
        }
    }

</script>


<style scoped>
    .result {
        height: 100vh;
        background-color: white;
        border-top: 1px solid blueviolet;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .infowindow {
        width: 75%;
        height: 75%;
        background-color: white;
        -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.50);
        -webkit-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.50);
        -moz-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.50);
        box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.50); 
        border-radius: 12px;
    }

    img {
        width: calc(100% - 10px);
        height: calc(100% - 6 * 12% - 6 * 2%);
        background-color: white;
        margin: 1% 5px 0 5px;
        -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.02);
        -webkit-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02);
        -moz-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02);
        box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02); 
        border-radius: 12px;
    }

    section {
        width: calc(100% - 10px);
        height: 12%;
        margin: 1% 5px 1% 5px;
        background-color: white;
        -webkit-box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.02);
        -webkit-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02);
        -moz-box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02);
        box-shadow: 5px 3px 44px 0px rgba(0,0,0,0.02); 
        border-radius: 12px;
    }
</style>