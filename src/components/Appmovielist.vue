<script>
import { store } from '../store.js'
import Appmoviecom from './Appmoviecom.vue'

export default {
    name: 'Appmovielist',
    data () {
    return {
      store
     };
    },
    components: {
        Appmoviecom
    }
}

</script>

<template>

<main>
    <div class="container">
        <div class="row">
            <Appmoviecom v-for="movie in store.movies" :key="movie.id"></Appmoviecom>
        </div>
    </div>
</main>

</template>

<style scoped lang="scss"></style>