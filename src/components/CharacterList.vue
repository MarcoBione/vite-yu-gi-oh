<template>
    <!-- single card -->
    <section>
        <div class="row">
            <CharacterCard v-for="(character, index) in store.characterList" :key="index" :character="character" />
        </div>
    </section>
</template>

<script>
import { store } from '../store';
import axios from 'axios';
import CharacterCard from './CharacterCard.vue';

export default {

    name: 'CharacterList',
    components: {
        CharacterCard,
    },

    data() {
        return {
            store,
        }
    },

}
</script>

<style lang="scss" scoped></style>