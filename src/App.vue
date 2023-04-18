<template>
  <div>
    <HeaderComponent />
    <MainComponent />
  </div>
</template>

<script>
import axios from 'axios';
import { store } from './store';
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';

export default {

  name: 'App',
  components: {
    HeaderComponent,
    MainComponent
  },

  data() {
    return {
      store
    }
  },

  methods: {
    getData() {
      const URL = store.URL + store.endpoint;
      axios.get(URL).then((res) => {
        store.characterList = res.data;
        console.log(store.characterList.data);
      });
    }
  },

  mounted() {
    store.endpoint = 'character';
    this.getData();
  }

}
</script>

<style lang="scss" scoped></style>