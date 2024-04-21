<script>

export default {
    name: 'Appmoviecom',
    props: {
        cardInfo: Object
    }
}

</script>

<template>

<div class="container">
    <div class="row">
        <img src="" alt="">

        <div class="ms-titolo">Titolo: {{ cardInfo.title }} </div>
        <div class="ms-or-titolo">Titolo Originale: {{ cardInfo.original_title }}</div>
        <div class="ms-lingua">Lingua Originale: {{ cardInfo.original_language }}</div>
        <div class="ms-voto">Voto: {{ cardInfo.vote_average }}</div>
    </div>
</div>

</template>

<style scoped lang="scss"></style>