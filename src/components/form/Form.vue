<template>
    <div>
        <form @submit="enviarFormulario($event)">
           <InputTextForm/>
           <InputTextForm/>
           <SubmitForm/>
        </form>
    </div>
</template>


<script>
import InputTextForm from './InputTextForm.vue'
import SubmitForm from './SubmitForm.vue'

export default {
    name: 'Form',
    components: {
        InputTextForm, 
        SubmitForm
    },
    methods: {
        enviarFormulario(e) {
            e.preventDefault();
            
            alert('Formulario enviado');
        }
    },
}
</script>