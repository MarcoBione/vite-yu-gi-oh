<template>
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 my-2">
        <div class="_myygocard text-center">
            <img :src="character.card_images[0].image_url" :alt="character.card_images.image_url">
            <h4>{{ character.name }}</h4>
            <div>{{ character.type }}</div>
            <div class="font-weight-bold">{{ character.archetype }}</div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'CharacterCard',
    props: ['character'],
}
</script>

<style lang="scss" scoped>
img {
    width: 200px;
}
</style>