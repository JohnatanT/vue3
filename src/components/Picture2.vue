<template>
    <div>
        <img :src="avatar" :alt="decricao">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
    
</template>

<script>
import MudarImagem from './MudarImagem.vue'

export default {
    name: 'Picture2',
    data() {
        return {
            avatar: require('@/assets/logo.png'),
            decricao: "logo Vue"
        }
    },
    components: {
        MudarImagem
    },
    methods: {
        trocarImagem() {
            alert('Trocou')
        }
    },
}
</script>