<script>

import Appheader from './components/Appheader.vue';
import Appmovielist from './components/Appmovielist.vue'


export default {
  components: {
    Appheader,
    Appmovielist
  },
  methods: {
    getMoviesFromApi() {

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
