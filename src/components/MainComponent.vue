<template>
    <div>

    </div>
</template>

<script>

axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=50&offset=0').then((res) => {
    console.log(res.data);
});

console.log(cards);
export default {
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped></style>