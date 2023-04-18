<template>
    <main>

        <div class="container">
            <CharacterListVue />
        </div>

        <div class="container">

        </div>

    </main>
</template>

<script>
import { store } from '../store';
import axios from 'axios';

import CharacterListVue from './CharacterList.vue';

export default {

    data() {
        return {
            store,
        }
    },
    components: {
        CharacterListVue,
    }

}
</script>

<style lang="scss" scoped></style>