<template>
    <!-- single card -->
    <section>
        <div class="row">
            <CharacterCard />
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

        }
    },

}
</script>

<style lang="scss" scoped></style>