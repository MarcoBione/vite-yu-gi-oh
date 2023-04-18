<template>
    <select class="form-select">
        <option selected value="scegli">Scegli</option>
        <option v-for="type, index in store.characterList.archetype" :value="type"></option>
    </select>
</template>

<script>
import { store } from '../store';
import axios from 'axios';

export default {
    name: 'SearchBar',
    data() {
        return {
            store,
        }
    },

}
</script>

<style lang="scss" scoped></style>