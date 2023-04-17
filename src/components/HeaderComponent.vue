<template>
    <div>

        <header class="d-flex align-item-center p-4 border border-1">
            <img class="_mylogo" src="	https://www.yugioh-card.com/eu/wp-content/themes/yugioh/images/logo/Yugioh-EN-DE.svg"
                alt="YuGiOh-Logo">
            <h1 class="_mytitle m-0">{{ title }}</h1>
        </header>

    </div>
</template>

<script>
export default {
    data() {
        return {
            title: 'Yu-Gi-Oh Api Deck',
        }
    }
}
</script>

<style lang="scss" scoped></style>