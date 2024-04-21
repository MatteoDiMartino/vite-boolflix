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
        <div class="ms-titolo">Titolo: {{ cardInfo.title }} </div>
        <div class="ms-or-titolo">Titolo Originale: {{ cardInfo.original_title }}</div>
        <div class="ms-lingua">[Lingua]</div>
        <div class="ms-voto">[Voto]</div>
    </div>
</div>

</template>

<style scoped lang="scss"></style>