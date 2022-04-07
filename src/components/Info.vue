<template>
    <div>
        <p v-if="trabalhando">Trabalhando...</p>
        <p v-else>Não estou trabalhando </p>
        <p>Usando VueJS 3!!</p>

        <button @click="showEmail">Mostrar e-mail</button>

        <p>Para acessar meu portifolio clique aqui <a v-bind:href="meu_link">AQUI</a> </p>
        <Picture2/>
    </div>
</template>


<script>
import Picture2 from './Picture2.vue'

export default {
    name: 'Info',
    data() {
        return {
            trabalhando: true,
            meu_link: '#'
        }
    },
    components: {
        Picture2
    },
    methods: {
        showEmail() {
            alert('Olá...');
        }
    },
}
</script>