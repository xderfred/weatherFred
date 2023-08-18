<template>
  <div class="cards">
    <section class="card" v-for="city in cities" v-bind:key="city.id">
      {{ city.name }}
    </section>
  </div>
</template>

<script>

import { ref } from "vue"
// import City from "../models/CityModel"

export default {

  setup() {
      const cities = ref([
        
        {name: "Berlin", temperature: 30},
        {name: "Moskau", temperature: 15},
        {name: "New York", temperature: 25},
        {name: "Rio", temperature: 33},
        {name: "Rome", temperature: 22},
        {name: "Paris", temperature: 17}
      ])


    return {
      cities
    }
  },

  name: 'CityCardsView',
  props: {
    msg: String
  }
}
</script>


<style scoped>

  .cards {
    display: flex;
    flex-wrap: nowrap;
    overflow-x: auto;
    height: 100vh;
    /* justify-content: center; */
    align-items: center;
    -webkit-overflow-scrolling: touch;
  }

  .cards::-webkit-scrollbar {
    display: none;
  }

  .card {
    height: 500px;
    width: 80%;
    margin: 50px;
    border-radius: 12px;
    box-shadow: 10px 15px 29px 6px blueviolet;
    flex: 0 0 auto;
  }
</style>
