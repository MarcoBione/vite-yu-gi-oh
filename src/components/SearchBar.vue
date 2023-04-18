<template>
    <select class="form-select bg-transparent text-white w-25" v-model="store.archetype">
        <option selected value="scegli">Scegli</option>
        <option v-for="archetype in archetypeList" :value="archetype">{{ archetype }}</option>
    </select>
</template>

<script>
import { store } from '../store';

export default {
    name: 'SearchBar',
    data() {
        return {
            store,
        }
    },
    computed: {
        archetypeList() {
            return new Set(this.store.characterList.filter((character) => {
                return character.archetype !== undefined;
            }).map((character) => character.archetype));
        }
    }

}
</script>

<style lang="scss" scoped>
option {
    background-color: #11001cff;
}
</style>