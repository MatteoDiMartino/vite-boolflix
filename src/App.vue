<script>
import { store } from './store.js'
import axios from 'axios';
import Appheader from './components/Appheader.vue';
import Appmovielist from './components/Appmovielist.vue'


export default {
  components: {
    Appheader,
    Appmovielist
  },
  data () {
    return {
      store
    };
  },
  methods: {
    getMoviesFromApi() {
      const queryParams = {
        api_key: store.apiKey,
        query: 'ritorno'
      };

      axios.get('https://api.themoviedb.org/3/search/movie', {
        params: queryParams
      }).
      then((response) => {
        store.movies = response.data.results;
      })
    },
  },
  mounted(){
    this.getMoviesFromApi();
  }
}
</script>

<template>

<Appheader></Appheader>
<Appmovielist></Appmovielist>


</template>

<style lang="scss">
@use './style/generic.scss'
</style>
