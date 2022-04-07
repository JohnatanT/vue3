<template>
    <img :src="avatar" :alt="decricao">
</template>

<script>
export default {
    name: 'Picture2',
    data() {
        return {
            avatar: require('@/assets/logo.png'),
            decricao: "logo Vue"
        }
    }
}
</script>