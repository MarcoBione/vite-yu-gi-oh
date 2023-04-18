<template>
    <select class="form-select bg-transparent text-white w-25">
        <option selected value="scegli">Scegli</option>
        <option v-for="type, index in store.characterList" :value="type.archetype">{{ type.archetype }}</option>
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

<style lang="scss" scoped>
option {
    background-color: #11001cff;
}
</style>