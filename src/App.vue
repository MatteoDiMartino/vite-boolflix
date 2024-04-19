<script>

import Appheader from './components/Appheader.vue';
import Appmovielist from './components/Appmovielist.vue'

export default {
  components: {
    Appheader,
    Appmovielist
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
