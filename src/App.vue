<template>
  <HeaderView/>
  <SearchView/>
  <CityCardsView/>
  <ResultView />
  <FooterView/>
</template>

<script>
import HeaderView from './components/HeaderView.vue';
import FooterView from './components/FooterView.vue'
import SearchView from './components/SearchView.vue';
import CityCardsView from './components/CityCardsView.vue';
import ResultView from './components/ResultView.vue';

export default {
  name: 'App',
  components: {
    HeaderView,
    FooterView,
    SearchView,
    CityCardsView,
    ResultView
}
}
</script>

<style>
#app {
    * {
      margin: 0;
      padding: 0;
    }
}

body {
  margin: 0;
}
</style>
