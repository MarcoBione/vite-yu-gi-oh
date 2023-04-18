<template>
    <main>

        <div class="container">
            <SearchBar />
        </div>

        <div class="container">
            <CharacterListVue />
        </div>

    </main>
</template>

<script>
import { store } from '../store';
import axios from 'axios';

import CharacterListVue from './CharacterList.vue';
import SearchBar from './SearchBar.vue';

export default {

    data() {
        return {
            store,
        }
    },
    components: {
        CharacterListVue,
        SearchBar,
    }

}
</script>

<style lang="scss" scoped></style>