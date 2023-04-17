<template>
    <div>

    </div>
</template>

<script>
import axios from 'axios';
axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=50&offset=0').then((res) => {
    console.log(res.data);
})
export default {
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped></style>