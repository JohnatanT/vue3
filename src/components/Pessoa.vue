<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{nome}}</h2>
        <Info :compEmail="email" />
    </div>
</template>

<script>
import Info from './Info.vue'

export default {
    name: 'Pessoa',
    components: {
        Info
    },
    data() {
        return {
            nome: 'Johnatan',
            email: 'teste@teste.com'
        }
    }
}
</script>